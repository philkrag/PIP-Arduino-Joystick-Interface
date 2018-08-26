
/*
// /////////////////////////////////////////////////////////////////////// COPYRIGHT NOTICE
// This program is free software: you can redistribute it and/or modify
// it under the terms of the GNU General Public License as published by
// the Free Software Foundation, either version 3 of the License, or
// (at your option) any later version.
// This program is distributed in the hope that it will be useful,
// but WITHOUT ANY WARRANTY; without even the implied warranty of
// MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
// GNU General Public License for more details.
// You should have received a copy of the GNU General Public License
// along with Pip-Project.  If not, see <http://www.gnu.org/licenses/>.
// /////////////////////////////////////////////////////////////////////// COPYRIGHT NOTICE
// /////////////////////////////////////////////////////////////////////// VERSION CONTROL
// PAGE CREATED BY: Phillip Kraguljac
// PAGE CREATED DATE: 2018-08-27
// DATE       || NAME           || MODIFICATION
// 2018-08-27   || Phillip Kraguljac    || Created.
// /////////////////////////////////////////////////////////////////////// VERSION CONTROL
*/

int Push_JS_Pin = 12;
int X_Axis_JS_Pin = A0;
int Y_Axis_JS_Pin = A1;
bool Push_JS_Value = 0;
int X_Axis_JS_Value = 0;
int Y_Axis_JS_Value = 0;
String Serial_Output = "";
String Joiner = ":";

void setup() {
Serial.begin(9600);
pinMode(Push_JS_Pin, INPUT_PULLUP);
}

void loop() {
Serial_Output = "";
Push_JS_Value = digitalRead(Push_JS_Pin);
X_Axis_JS_Value = analogRead(X_Axis_JS_Pin);
Y_Axis_JS_Value = analogRead(Y_Axis_JS_Pin);

Serial_Output = String(Push_JS_Value)+Joiner+String(X_Axis_JS_Value)+Joiner+String(Y_Axis_JS_Value);

Serial.println(Serial_Output);

delay(100);

}
