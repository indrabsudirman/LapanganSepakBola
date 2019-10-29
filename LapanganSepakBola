import java.awt.Color;
import java.awt.Font;
import java.awt.Graphics;
import java.awt.Graphics2D;
import java.awt.BasicStroke;

import javax.swing.JFrame;
import javax.swing.JPanel;

public class LapanganSepakBola extends JPanel {

  public void paintComponent(Graphics graphics) {
    super.paintComponent(graphics);
    Graphics2D graphics2D = (Graphics2D) graphics;
    Color lightGreen, darkGreen, lightBrown;

    lightGreen = new Color (0, 255, 0);
    darkGreen = new Color (19, 226, 19);
    lightBrown = new Color (218, 106, 0 );
    graphics2D.setColor(lightGreen);
    graphics2D.fillRect(0,0,1280,776);
    
    graphics2D.setStroke(new BasicStroke(50));
    graphics2D.setColor(darkGreen);
    graphics2D.drawOval(185, -67, 910, 910);
    graphics2D.setColor(darkGreen);
    graphics2D.drawOval(285, 33, 710, 710);
    graphics2D.setColor(darkGreen);
    graphics2D.drawOval(385, 133, 510, 510);
    graphics2D.setColor(lightGreen);
    graphics2D.drawOval(435, 183, 410, 410);
    graphics2D.setColor(darkGreen);
    graphics2D.drawOval(485, 233, 310, 310);
    graphics2D.setColor(lightGreen);
    graphics2D.drawOval(535, 283, 210, 210);
    graphics2D.setColor(darkGreen);
    graphics2D.drawOval(585, 333, 110, 110);
    
    
    graphics2D.setColor(Color.white);
    int appW = getSize().width; //1280
    int appH = getSize().height; //776
    
    
    graphics2D.setStroke(new BasicStroke(2.0f));
    graphics2D.drawRect(200,88,880,600); //perbandingan 8 satuan 110 x 75 = 880,600 nilai dari 200 dari selisih (1280 - 880)/2. nilai 88 dari (776 - 600)/2
    graphics2D.drawOval(585,333,110,110); //nilai 233 dari titik tengah (776:2) = 388. 388 - (310:2). Nilai 485 dari (1280:2) = 640. 640 - (310:2) 
    graphics2D.drawRect(200,278,140,220); //kotak besar gawang kiri
    graphics2D.drawRect(940,278,140,220); //kotak besar gawang kanan
    graphics2D.drawRect(200,318,80,140); //kotak besar gawang kiri kecil pinalti
    graphics2D.drawRect(1000,318,80,140); //kotak besar gawang kanan kecil pinalti
    graphics2D.drawArc(310,358,60,60,90, -180); //kotak besar gawang kiri kecil pinalti
    graphics2D.drawArc(910,358,60,60,90, 180); //kotak besar gawang kanan kecil pinalti
    graphics2D.drawRect(160,338,40,100); //kotak kecil luar gawang kiri kecil pinalti
    graphics2D.drawRect(1080,338,40,100); //kotak kecil luar gawang kanan kecil pinalti
    graphics2D.drawLine(640, 88, 640, 688); //garis tengah
    
    graphics2D.drawArc(200, 88, 10, 10, 45, -225); //arc kecil pojok kiri atas
    graphics2D.drawArc(200, 678, 10, 10, -45, 225); //arc kecil pojok kiri bawah
    graphics2D.drawArc(1070, 88, 10, 10, 0, -225); //arc kecil pojok kanan atas
    graphics2D.drawArc(1070, 678, 10, 10, -90, -225); //arc kecil pojok kanan bawah
    
    graphics2D.setStroke(new BasicStroke(3.0f));
    graphics2D.drawOval(310, 388, 3,3); //titik bola pinalti kiri
    graphics2D.drawOval(967, 388, 3,3); //titik bola pinalti kanan
    graphics2D.drawOval(639, 385, 3,3); //titik bola tengah lapangan
    graphics2D.setColor(lightGreen);
    graphics2D.fillRect(0,0,1279,87); //rumput hijau luar lapangan atas
    graphics2D.fillRect(0,689,1258,88); //rumput hijau luar lapangan bawah
    graphics2D.fillRect(0,199,199,766); //rumput hijau luar lapangan kiri
    graphics2D.fillRect(1081,0,199,765); //rumput hijau luar lapangan kanan
    
    
    graphics2D.setColor(lightBrown);
    graphics2D.setStroke(new BasicStroke(20));
    graphics2D.drawRoundRect(170,58,940,660,20,20); //tanah runaway bawah
    graphics2D.drawRoundRect(160,48,960,680,20,20); //tanah runaway atas
    
    graphics2D.setColor(Color.white);
    graphics2D.setStroke(new BasicStroke(1.0f));
    graphics2D.drawRect(180,68,920,640); //garis runaway bawah
    graphics2D.drawRoundRect(170,58,940,660,20,20); // garis runaway no 1 dari bawah
    graphics2D.drawRoundRect(160,48,960,680,20,20); // garis runaway no 2 dari bawah
    graphics2D.drawRoundRect(150,38,980,700,33,33); // garis runaway no 3 dari bawah
    graphics2D.drawLine(640, 38, 640, 67); //garis start finish runaway
    
    Font calibriBold = new Font ("Calibri", Font.BOLD, 18);
    graphics2D.setFont(calibriBold);
    graphics2D.drawString("Lapangan Sepak Bola", 480, 26);
    Font calibri = new Font ("Calibri", Font.PLAIN, 18);
    graphics2D.setFont(calibri);
    graphics2D.drawString("dengan Java", 703, 26);

  }

  public static void main(String[] args) {
    LapanganSepakBola lapanganSepakBola = new LapanganSepakBola();
    JFrame frame = new JFrame("Lapangan Sepak Bola");
    frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    frame.add(lapanganSepakBola);
    frame.setExtendedState(JFrame.MAXIMIZED_BOTH);
    frame.setLocationRelativeTo(null);
    frame.setVisible(true);
  }
}
