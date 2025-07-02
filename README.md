# hourly-wage-expenses-calc
Public Class Form1
    Dim hours As Double
    Dim rate As Double
    Dim grossWages As Double
    Dim deductions As Double
    Dim netWages As Double
    Dim totalGross As Double
    Dim totalDeductions As Double
    Dim totalnetWages As Double
    Private sOperator As String





    Private Sub Label1_Click(sender As Object, e As EventArgs) Handles btnName.Click

    End Sub

    Private Sub Hoursworked_Click(sender As Object, e As EventArgs) Handles Hoursworked.Click

    End Sub

    Private Sub Label1_Click_1(sender As Object, e As EventArgs) Handles Label1.Click

    End Sub

    Private Sub Label6_Click(sender As Object, e As EventArgs) Handles Label6.Click

    End Sub

    Private Sub Label7_Click(sender As Object, e As EventArgs) Handles Label7.Click

    End Sub

    Private Sub Label8_Click(sender As Object, e As EventArgs) Handles Label8.Click

    End Sub

    Private Sub btnExit_Click(sender As Object, e As EventArgs) Handles btnExit.Click
        Me.Close()
    End Sub

    Private Sub Clear_Click(sender As Object, e As EventArgs) Handles Clear.Click
        txtName.Clear()
        txtHours.Clear()
        txtRate.Clear()
        txtGross.Clear()
        txtDed.Clear()
        txtNet.Clear()
        txtTotGross.Clear()
        txtTotDed.Clear()
        txtTotoNet.Clear()
        txtName.Focus()

    End Sub

    Private Sub txtName_TextChanged(sender As Object, e As EventArgs) Handles txtName.TextChanged

    End Sub

    Private Sub btnPaycheck_Click(sender As Object, e As EventArgs) Handles btnPaycheck.Click

        txtGross.Text = grossWages.ToString("$")
        txtDed.Text = deductions.ToString("$")
        txtNet.Text = netWages.ToString("$")

        txtGross.Text = (txtHours.Text * txtRate.Text).ToString("C")
        txtDed.Text = (txtGross.Text * 0.15).ToString("C")
        txtNet.Text = (txtGross.Text - txtDed.Text).ToString("C")



    End Sub

    Private Sub txtGross_TextChanged(sender As Object, e As EventArgs) Handles txtGross.TextChanged

    End Sub

    Private Sub btnTotals_Click(sender As Object, e As EventArgs) Handles btnTotals.Click
        txtTotGross.Text = totalGross.ToString("C")
        txtTotDed.Text = totalDeductions.ToString("C")
        txtTotoNet.Text = totalnetWages.ToString("C")

        txtTotGross.Text = (txtHours.Text * txtRate.Text).ToString("C")
        txtTotDed.Text = (txtTotGross.Text * 0.15).ToString("C")
        txtTotoNet.Text = (txtTotGross.Text - txtTotDed.Text).ToString("C")
    End Sub

    Private Sub Label4_Click(sender As Object, e As EventArgs) Handles Label4.Click

    End Sub
End Class
