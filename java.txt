public class Main {

    public static void main(String[] args)
    {
        f( 168260271);
        f(  27364375);
        f(  67294091);
    }
    public static int f(int worldTimex)
    {
        int year = worldTimex/(1440*365)+ 1;
        int day = (worldTimex/1440)%365+1;
        int hour= (worldTimex/60)%24;
        int minute= worldTimex%60;
        int tramel= (worldTimex/1440)%9;
        int felucca= (worldTimex/1440)%14;

        System.out.println("worldTime = " + worldTimex);
        System.out.printf("It is %d:%02d on day %d of the year %d. ", hour,minute,day,year);
        System.out.println("\nTramel is in day " + (tramel+1) + " of its 9 day phase.");
        System.out.println("Felucca is in day " + (felucca +1) + " of its 14 day phase.\n");

        return 0;

    }
}
