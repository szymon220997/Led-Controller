# Led-Controller
All rights reserved

$regfile = "m8def.dat"
$crystal = 1000000

Config Portb = &B11111111 : Portb = &B00000000
Config Portc = &B00000000 : Portc = &B00000000
Config Timer1 = Pwm , Pwm = 8 , Prescale = 1 , Compare A Pwm = Clear Up , Compare B Pwm = Clear Up
Config Adc = Single , Prescaler = Auto , Reference = Avcc

Start Adc
Dim Gaz As Word
Pwm1a = 0
Pwm1b = 0


Do
Gaz = Getadc(0)



If Gaz < 100 And Gaz > 99 Then
Pwm1a = 255
End If


If Gaz < 98 And Gaz > 97 Then
Pwm1a = 245
End If


If Gaz < 96 And Gaz > 95 Then
Pwm1a = 235
End If


If Gaz < 94 And Gaz > 93 Then
Pwm1a = 225
End If


If Gaz < 92 And Gaz > 91 Then
Pwm1a = 215
End If


If Gaz < 90 And Gaz > 89 Then
Pwm1a = 204
End If


If Gaz < 88 And Gaz > 87 Then
Pwm1a = 194
End If


If Gaz < 86 And Gaz > 85 Then
Pwm1a = 184
End If


f Gaz < 84 And Gaz > 83 Then
Pwm1a = 174
End If


If Gaz < 82 And Gaz > 81 Then
Pwm1a = 163
End If


If Gaz < 80 And Gaz > 79 Then
Pwm1a = 153
End If


If Gaz < 78 And Gaz > 77 Then
Pwm1a = 143
End If


If Gaz < 76 And Gaz > 75 Then
Pwm1a = 133
End If


If Gaz < 74 And Gaz > 73 Then
Pwm1a = 122
End If


If Gaz < 72 And Gaz > 71 Then
Pwm1a = 112
End If


If Gaz < 70 And Gaz > 69 Then
Pwm1a = 102
End If


If Gaz < 68 And Gaz > 67 Then
Pwm1a = 92
End If


If Gaz < 66 And Gaz > 65 Then
Pwm1a = 81
End If


If Gaz < 64 And Gaz > 63 Then
Pwm1a = 71
End If


If Gaz < 62 And Gaz > 61 Then
Pwm1a = 61
End If


If Gaz < 60 And Gaz > 59 Then
Pwm1a = 51
End If


If Gaz < 58 And Gaz > 57 Then
Pwm1a = 40
End If



If Gaz < 56 And Gaz > 55 Then
Pwm1a = 30
End If



If Gaz < 54 And Gaz > 53 Then
Pwm1a = 20
End If



If Gaz < 52 And Gaz > 51 Then
Pwm1a = 10
End If


If Gaz < 50 And Gaz > 49 Then
Pwm1a = 0
End If


Loop
End
