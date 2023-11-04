
import net.glxn.qrgen.core.image.ImageType;
import net.glxn.qrgen.javase.QRCode;

public class QRCodeGenerator {
    public static void main(String[] args) {
        String data = "Hello, World!";
        QRCode.from(data).to(ImageType.PNG).withSize(300, 300).writeTo(new FileOutputStream("my_qr_code.png"));
    }
}
