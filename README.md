import java.io.File;
import java.io.FileReader;
import java.io.IOException;


public class Jala {
	public static void main(String[] args) throws IOException {
		File file = new File("myfile.txt");
		FileReader fr = new FileReader(file);
        try
        {
            int data;
            while ((data = fr.read()) != -1) {
                System.out.print((char)data);
            }
        } catch (IOException e) {
            System.out.println("Sorry!!! can't read the file");;
        }
        
      }
}
