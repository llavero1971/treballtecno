#define E1 10  // Enable Pin for motor 1
#define E2 11  // Enable Pin for motor 2
 
#define I1 8  // Control pin 1 for motor 1
#define I2 9  // Control pin 2 for motor 1
#define I3 12  // Control pin 1 for motor 2
#define I4 13  // Control pin 2 for motor 2
 
void setup() {
 
    pinMode(E1, OUTPUT);
    pinMode(E2, OUTPUT);
    pinMode(I3, OUTPUT);
    pinMode(I4, OUTPUT);
    pinMode(I1, OUTPUT);
    pinMode(I2, OUTPUT);
}
 

  /* HIGH
    analogWrite(E2, 100); 
    digitalWrite(I4, );
    digitalWrite(I3, LOW);
    delay(2000);
    analogWrite(E2, 255);
    delay(2000);
   */   





llllllllllllllllllllllllllllll

#define E1 10  // Enable Pin for motor 1
#define E2 11  // Enable Pin for motor 2
 
#define I1 8  // Control pin 1 for motor 1
#define I2 9  // Control pin 2 for motor 1
#define I3 12  // Control pin 1 for motor 2
#define I4 13  // Control pin 2 for motor 2
 
void setup() {
 
    pinMode(E1, OUTPUT);
    pinMode(E2, OUTPUT);
    pinMode(I3, OUTPUT);
    pinMode(I4, OUTPUT);
    pinMode(I1, OUTPUT);
    pinMode(I2, OUTPUT);
}

void loop() {

//ràpid
analogWrite(E2,0);
  analogWrite(E1, 0);
  delay(100);

  
    analogWrite(E2, 255); // Run in full speed
 
    digitalWrite(I4, HIGH);
    digitalWrite(I3, LOW);
        
    analogWrite(E1, 255); // Run in full speed

    digitalWrite(I2, HIGH);
    digitalWrite(I1, LOW);

//ara a velocitat lenta

  analogWrite(E2, 0);
  analogWrite(E1, 0);
  delay(100);
  
analogWrite(E2, 153); // Run in medium speed
 
    digitalWrite(I4, HIGH);
    digitalWrite(I3, LOW);
        
    analogWrite(E1, 153); // Run in full speed

    digitalWrite(I2, HIGH);
    digitalWrite(I1, LOW);
    
}
