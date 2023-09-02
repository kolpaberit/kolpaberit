- 👋 Hi, I’m @kolpaberit</strong></summary>

👀 Studying robotics to create machines of the future. Robotics is my passion! 🤖🔧
🌱 I’m currently learning about robotic systems, automation, and artificial intelligence.
💞️ I’m open to collaborating on projects involving robotics and autonomous systems.
📫 You can reach me via email: kolpaberit@gmail.com
</details>

Sample Repository: Simple Line Following Robot with Arduino

```arduino
int leftSensor = 2;
int rightSensor = 3;
int leftMotor = 9;
int rightMotor = 10;

void setup() {
  pinMode(leftSensor, INPUT);
  pinMode(rightSensor, INPUT);
  pinMode(leftMotor, OUTPUT);
  pinMode(rightMotor, OUTPUT);
}

void loop() {
  if (digitalRead(leftSensor) == HIGH && digitalRead(rightSensor) == LOW) {
    digitalWrite(leftMotor, HIGH);
    digitalWrite(rightMotor, LOW);
  } else if (digitalRead(leftSensor) == LOW && digitalRead(rightSensor) == HIGH) {
    digitalWrite(leftMotor, LOW);
    digitalWrite(rightMotor, HIGH);
  } else {
    digitalWrite(leftMotor, HIGH);
    digitalWrite(rightMotor, HIGH);
  }
}
