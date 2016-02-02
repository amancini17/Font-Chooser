#FontChooser
import java.applet.Applet;

import java.awt.FlowLayout;
import java.awt.GraphicsEnvironment;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;

import java.awt.Font;
import java.awt.Color;
import java.awt.Dimension;
import java.awt.Image;
import java.awt.BorderLayout;

import javax.swing.SwingUtilities;

import java.swing.ImageIcon;
import javax.swing.JFrame;
import javax.swing.JPanel;
import javax.swing.JLabel;
import javax.swing.JComboBox;
import javax.swing.JColorChooser;
import javax.swing.JTextArea;

import java.swing.border.LineBorder;


public class FontChooser extends JFrame implements Action Listener
   {
   JLabel fontSample = new JLabel(
   "The quick brown fox jumped over the lazy dog’s back.
    Pack my box with five dozen liquor jugs.
    Jackdaws love my big sphinx of quartz.
    Mr. Jock, TV quiz PhD, bags few lynx.
    abcdefghijklmnopqrstuvwxyz
    ABCDEFGHIJKLMNOPQRSTUVWXYZ
    01234567890
    €†™´¸¢©¤°÷½¼¾>¡¿«‘’<¯µ ·¬ªº¶±£"»®§­¹²³ß×™¨¥
    ÀÁÂÃÄÅÆÇÈÉ ÊËÌÍÎÏÐÑÒÓÔ ÕÖØÙÚÛÜÝÞÿ
    àáâãäåæçèé êëìíîïðñòóô õöøùúûüýþÿ
    !"#$%&'()*+,-./:;<=>?@[\^_z{|}~
    uvw wW gq9 2z 5s il17|!j oO08 `'" ;:,. m nn rn {[()]}u");
   
   
   public static void main ( String [] args )
      {
      GraphicsEnvironment ge = GraphicsEnvironment.getLocalGraphicsEnvironment();
      String[] names = ge.getAvailableFontFamilyNames();
      for ( int i=0; i<names.length; i++ )
         {
             System.out.println( names[i] );
         }
      }
}
