<div align="center">

## A very simple Encrypt and Unencrypt


</div>

### Description

This is a very simple encrypt/unenceypt and when i say simple i mean simple. works for any string containg the normal chr's ie. (1-9,a-z). Works good tho for simple encrypt.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[DoWnLoHo](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/downloho.md)
**Level**          |Unknown
**User Rating**    |4.2 (161 globes from 38 users)
**Compatibility**  |VB 3\.0, VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[String Manipulation](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/string-manipulation__1-5.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/downloho-a-very-simple-encrypt-and-unencrypt__1-3860/archive/master.zip)





### Source Code

```
Function Eyncrypt(sData As String) As String
Dim sTemp as String, sTemp1 as String
For iI% = 1 To Len(sData$)
  sTemp$ = Mid$(sData$, iI%, 1)
  lT = Asc(sTemp$) * 2
  sTemp1$ = sTemp1$ & Chr(lT)
Next iI%
Eyncrypt$ = sTemp1$
End Function
Function UnEyncrypt(sData As String) As String
Dim sTemp as String, sTemp1 as String
For iI% = 1 To Len(sData$)
  sTemp$ = Mid$(sData$, iI%, 1)
  lT = Asc(sTemp$) \ 2
  sTemp1$ = sTemp1$ & Chr(lT)
Next iI%
UnEyncrypt$ = sTemp1$
End Function
```

