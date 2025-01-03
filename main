const int tempPin = A0; // Analog pin connected to LM35

void setup() {
  Serial.begin(9600); // Initialize serial communication at 9600 baud
  Serial.println("Temperature Sensor Initialized");
}

void loop() {
  int analogValue = analogRead(tempPin); // Read the analog value from LM35
  float voltage = analogValue * (5.0 / 1023.0); // Convert to voltage
  float temperatureC = voltage * 100.0; // Convert voltage to Celsius

  Serial.print("Temperature: ");
  Serial.print(temperatureC);
  Serial.println(" °C"); // Print temperature in Celsius
  
  delay(1000); // Wait for 1 second before the next reading
}
