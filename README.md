package tugasbesar_praktikum_daa;
public class No2 {
public static void main(String[] args) {
        int[] cinta = {150, 162, 170, 155, 140};
        codeBaper(cinta);
        selaluSayang(cinta);
    }
    
    public static void codeBaper(int[] kita){
        for(int aku=1; aku<kita.length; aku++){
            int kamu, dia;
            kamu = aku-1;
            dia = kita[aku];
            while(kamu>=0 && kita[kamu]>dia){
                kita[kamu+1] = kita[kamu];
                kamu--;
            }
            kita[kamu+1] = dia;
        }
    }
    
    
    public static void selaluSayang(int[] kamu){
        for(int putus=0; putus<kamu.length; putus++){
            System.out.print(kamu[putus] + " ");
        }
        System.out.println();
    }
}
