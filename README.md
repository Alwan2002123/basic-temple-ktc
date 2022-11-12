*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author M.Alwan Algifari
 */
public abstract class BangunDatar {
    String warna;
    
    String getWarna() {
        return warna;
    }
    
    void setWarna(String warna) {
        this.warna = warna;
    }
    
    abstract float getLuas();
}


/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author M.Alwan Algifari
 */
public class Lingkaran extends BangunDatar{

    float jari_jari;
    
    public Lingkaran(float jari_jari){
        this.jari_jari = jari_jari;
    }
    
    @Override
    float getLuas() {
        return (float) Math.PI * jari_jari * jari_jari;
    }
    
}


/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author M.Alwan Algifari
 */
public class Main {
    public static void main(String[] args) {
        
        BangunDatar segitiga = new SegiTiga(12,20);
        BangunDatar lingkaran = new Lingkaran(60);
        
        System.out.println("Luas dari bangun datar segitiga : " + segitiga.getLuas());
        System.out.println("Luas dari bangun datar lingkaran : " + lingkaran.getLuas());
    }
}


/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author M.Alwan Algifari
 */
public class SegiTiga extends BangunDatar {
    private float alas;
    private float tinggi;
    
    public SegiTiga(float alas, float tinggi){
        this.alas = alas;
        this.tinggi = tinggi;
    }
    
    @Override
    float getLuas() {
        return (float)0.5 * alas * tinggi;
    }
}
Footer
© 2022 GitHub, Inc.
Footer navigation


/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author M.Alwan Algifari
 */
public class Main {
    public static void main(String[] args) {
        
        BangunDatar segitiga = new SegiTiga(12,20);
        BangunDatar lingkaran = new Lingkaran(60);
        
        System.out.println("Luas dari bangun datar segitiga : " + segitiga.getLuas());
        System.out.println("Luas dari bangun datar lingkaran : " + lingkaran.getLuas());
    }
}


/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author M.Alwan Algifari
 */
public class SegiTiga extends BangunDatar {
    private float alas;
    private float tinggi;
    
    public SegiTiga(float alas, float tinggi){
        this.alas = alas;
        this.tinggi = tinggi;
    }
    
    @Override
    float getLuas() {
        return (float)0.5 * alas * tinggi;
    }
}
