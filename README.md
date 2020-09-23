<div align="center">

## Creating a WYSIWYG HTML Editor with 4 lines of code\.


</div>

### Description

As the user is typing the HTML code, it is updated in the web browser control immediately. Great for an HTML Editor or just for testing out code.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Syllva Tech Software](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/syllva-tech-software.md)
**Level**          |Beginner
**User Rating**    |4.0 (16 globes from 4 users)
**Compatibility**  |VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[Internet/ HTML](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/internet-html__1-34.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/syllva-tech-software-creating-a-wysiwyg-html-editor-with-4-lines-of-code__1-30453/archive/master.zip)





### Source Code

To make a WYSIWYG HTML editor, simply put a textbox and a web browser control (here named wb) on a form. Add a module to the project and put in the following code:<P>
Sub Render()<P>
  wb.Document.Script.Document.Clear<BR>
  wb.Document.Script.Document.Write Text1.text<BR>
  wb.Document.Script.Document.Close<BR>
  Exit Sub<P>
End Sub<P>
To use it, place this in the textbox's KeyPress or Change event (see below for details on this choice) event:<P>Render<P>
Simple, isn't it? Now you can view your HTML code as you type it. It helps you to test out your HTML before putting it on your real page. Or you can use this in an actual editor to provide real-time previewing. <P>And since it uses Micro$oft's web browser control, you can use HTML, CSS, JavaScript and ASP.<P>As mentioned above, this code can be used in the Textbox's Keypress or Change events. Use the Keypress event if you want to use it as a simple view-HTML-as-you-type kind of editor. If you're making an editor, place the <I>Render</I> in the Textbox's Change event to let the magic begin. If you want this in a project, I uploaded one<A HREF="http://www.planet-source-code.com/xq/ASP/txtCodeId.7489/lngWId.1/qx/vb/scripts/ShowCode.htm">here</A>.

