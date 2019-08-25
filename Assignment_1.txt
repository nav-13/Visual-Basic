Public Class Form1

    Dim output As Integer
    Dim roman As String

    Private Sub Label1_Click(sender As System.Object, e As System.EventArgs) Handles arabicInt.Click

    End Sub

    Private Sub NumericUpDown1_ValueChanged(sender As System.Object, e As System.EventArgs) Handles int1.ValueChanged

    End Sub

    Private Sub addButton_Click(sender As System.Object, e As System.EventArgs) Handles addButton.Click
        output = int1.Value + int2.Value
        roman = ""
        If output < 0 Then
            output = 0
        End If
        If output > 5000 Then
            output = 0
        End If
        arabicInt.Text = output
        While output >= 1000
            roman = roman + "M"
            output = output - 1000
        End While
        While output >= 900
            roman = roman + "CM"
            output = output - 900
        End While
        While output >= 500
            roman = roman + "D"
            output = output - 500
        End While
        While output >= 400
            roman = roman + "CD"
            output = output - 400
        End While
        While output >= 100
            roman = roman + "C"
            output = output - 100
        End While
        While output >= 90
            roman = roman + "XC"
            output = output - 90
        End While
        While output >= 50
            roman = roman + "L"
            output = output - 50
        End While
        While output >= 40
            roman = roman + "XL"
            output = output - 40
        End While
        While output >= 10
            roman = roman + "X"
            output = output - 10
        End While
        While output >= 9
            roman = roman + "IX"
            output = output - 9
        End While
        While output >= 5
            roman = roman + "V"
            output = output - 5
        End While
        While output >= 4
            roman = roman + "IV"
            output = output - 4
        End While
        While output >= 1
            roman = roman + "I"
            output = output - 1
        End While
        romanInt.Text = roman

    End Sub

    Private Sub Form1_Load(sender As System.Object, e As System.EventArgs) Handles MyBase.Load

    End Sub

    Private Sub subButton_Click(sender As System.Object, e As System.EventArgs) Handles subButton.Click
        output = int1.Value - int2.Value
        roman = ""
        If output < 0 Then
            output = 0
        End If
        If output > 5000 Then
            output = 0
        End If
        arabicInt.Text = output
        While output >= 1000
            roman = roman + "M"
            output = output - 1000
        End While
        While output >= 900
            roman = roman + "CM"
            output = output - 900
        End While
        While output >= 500
            roman = roman + "D"
            output = output - 500
        End While
        While output >= 400
            roman = roman + "CD"
            output = output - 400
        End While
        While output >= 100
            roman = roman + "C"
            output = output - 100
        End While
        While output >= 90
            roman = roman + "XC"
            output = output - 90
        End While
        While output >= 50
            roman = roman + "L"
            output = output - 50
        End While
        While output >= 40
            roman = roman + "XL"
            output = output - 40
        End While
        While output >= 10
            roman = roman + "X"
            output = output - 10
        End While
        While output >= 9
            roman = roman + "IX"
            output = output - 9
        End While
        While output >= 5
            roman = roman + "V"
            output = output - 5
        End While
        While output >= 4
            roman = roman + "IV"
            output = output - 4
        End While
        While output >= 1
            roman = roman + "I"
            output = output - 1
        End While
        romanInt.Text = roman
    End Sub
End Class
