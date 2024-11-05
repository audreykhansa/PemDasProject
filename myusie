# PemDasProject
import java.util.Scanner;

public class MoodSicApp {
    public static void main(String[] args) {
        Scanner musicYeehaw = new Scanner(System.in);

        // Daftar mood yang tersedia
        String[] moods = {"happy", "sad", "relaxed", "excited", "angry", "in love"};

        // Daftar bahasa yang tersedia
        String[] languages = {"english", "indonesia", "korea"};

        String[][] songsEng = {
            {""},

            {"Someone Like You - Adele", "Fix You - Coldplay"},

            {"Weightless - Marconi Union", "River Flows in You - Yiruma"},

            {"Out of the Old - Olivia Rodrigo",},

            {"In the End - Linkin Park", "Break Stuff - Limp Bizkit"},

            {"Little Things - One Direction",
            "I Think They Call This Love - Elliot James, Reay",
            "Call It What You Want - Taylor Swift"}
        };

        String[][] songsIndo = {
            {"Tujuh Belas - Tulus",
            "Menikmati Hariku - Sherina Munaf"},

            {"Diri - Tulus",
            "Jalan Pulang - Yura Yunita",
            "Duar Hidup - Donne Maula"},

            {"Weightless - Marconi Union", "River Flows in You - Yiruma"},

            {"Lekas - Tulus",},

            {},

            {"Jatuh Suka - Tulus",
            "Jendela Kelas Satu - Iwan Fals",
            "Satu-satunya - HIVI"}
        };

        String[][] songsKor = {
            {},

            {"Silent Cry - Stray Kids",
            "Encore - GOT7",
            "Hug - Seventeen"},

            {"Weightless - Marconi Union", "River Flows in You - Yiruma"},

            {"Don't Stop Me Now - Queen", "Can't Hold Us - Macklemore"},

            {},

            {"Sorry, I Love You - Stray Kids",
            "Love Wins All - IU",
            "LOCO - ITZY"}
        };

        // Meminta pengguna memasukkan mood terlebih dahulu
        System.out.println("Hey, this is Myusie. What are you feeling today? (happy, sad, relaxed, excited, angry, in love): ");
        String userMood = musicYeehaw.nextLine().toLowerCase();

        int moodIndex = -1;

        // Mencari indeks mood yang dimasukkan pengguna
        for (int i = 0; i < moods.length; i++) {
            if (userMood.equals(moods[i])) {
                moodIndex = i;
                break;
            }
        }

        // Jika mood tidak ditemukan, tampilkan pesan kesalahan dan keluar
        if (moodIndex == -1) {
            System.out.println("Coudln't find mood. Please try again.");
        } else {
            // Meminta pengguna memilih bahasa setelah mood dimasukkan
            System.out.println("Choose the language (english/indonesia/korea): ");
            String userLanguage = musicYeehaw.nextLine().toLowerCase();

            if (userLanguage.equals("english")) {
                System.out.println("Songs recommendations if you are " + userMood + ":");
                for (String song : songsEng[moodIndex]) {
                    System.out.println("- " + song);
                }
            } else if (userLanguage.equals("indonesia")) {
                System.out.println("Song recommendations if you are " + userMood + ":");
                for (String song : songsIndo[moodIndex]) {
                    System.out.println("- " + song);
                }
            } else if (userLanguage.equals("korea")) {
                System.out.println("Song recommendations if you are " + userMood + ":");
                for (String song : songsKor[moodIndex]) {
                    System.out.println("- " + song);
                }
            } else {
                System.out.println("Please try again...");
            }
        }

        musicYeehaw.close();
    }
}
