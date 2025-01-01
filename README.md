# Running-Text-LCD-I2C
#include <Wire.h>
#include <LiquidCrystal_I2C.h> 

const int kolom = 16; 
const int baris = 2;  
LiquidCrystal_I2C lcd(0x27, kolom, baris); 

void setup() {
  lcd.init();          
  lcd.backlight();     
  lcd.setCursor(0, 0);
  lcd.print("Docky Agresma"); 
}

void loop() {
  lcd.setCursor(0, 0); 
  lcd.print("Docky Agresma!"); 
  delay(1000);         
  lcd.clear();         
}
