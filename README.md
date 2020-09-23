<div align="center">

## Real IP Finder


</div>

### Description

When you use winsock to find your ip address, it will return you the ip of your internal network (if you have one). So this simple code is useful to find your real ip (the ip you use when connected to the internet).
 
### More Info
 
This is a simple code, to see it in action, you need to have a Winsock control in your component choices, and place it in your form and name it "Winsock".


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[James Salim](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/james-salim.md)
**Level**          |Beginner
**User Rating**    |4.0 (16 globes from 4 users)
**Compatibility**  |VB 5\.0, VB 6\.0
**Category**       |[Internet/ HTML](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/internet-html__1-34.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/james-salim-real-ip-finder__1-11329/archive/master.zip)





### Source Code

```
Private Sub Form_Load()
  Winsock.Connect "www.microsoft.com", 80
End Sub
Private Sub Winsock_Connect()
  MsgBox "Your Real IP is: " + Winsock.LocalIP, vbOKOnly, "Real IP"
  Winsock.Close
End Sub
```

