<!-- default file list -->
*Files to look at*:

* [HomeController.cs](./CS/Controllers/HomeController.cs) (VB: [HomeController.vb](./VB/Controllers/HomeController.vb))
* [MyItem.cs](./CS/Models/MyItem.cs) (VB: [MyItem.vb](./VB/Models/MyItem.vb))
* [Script.js](./CS/Scripts/Script.js) (VB: [Script.js](./VB/Scripts/Script.js))
* [GridViewPartial.cshtml](./CS/Views/Home/GridViewPartial.cshtml)
* [Index.cshtml](./CS/Views/Home/Index.cshtml)
<!-- default file list end -->
# How to perform GridView instant updating using different editors in the DataItem template 
<!-- run online -->
**[[Run Online]](https://codecentral.devexpress.com/e3326/)**
<!-- run online end -->


<p><strong>UPDATED:</strong><br /><br />Starting with version 13.2, the GridView control offers the basic "Batch Editing Mode" functionality that allows accomplishing a similar task with less effort and does not require so much extra code. See the <a href="https://community.devexpress.com/blogs/aspnet/archive/2013/12/16/asp-net-webforms-amp-mvc-gridview-batch-edit-what-39-s-new-in-13-2.aspx">ASP.NET WebForms & MVC: GridView Batch Edit </a>blog post to learn more about this new functionality.<br />Starting with version 14.1, the GridView control offers advanced "Batch Editing Mode" programming options.<br /><br />You can find a standalone DB-independent solution in our Code Examples base at:<br /><a href="https://www.devexpress.com/Support/Center/p/E5046">GridView - A simple Batch Editing implementation</a> <br /><br />If you have version v14.1+ available, consider using the built-in functionality instead of the approach detailed below.<br />If you need further assistance with this functionality, please create a new ticket in our Support Center.<br /><br />The example illustrates a functionality similar to that demonstrated in the <a href="https://www.devexpress.com/Support/Center/p/E2333">How to perform ASPxGridView instant updating using different editors in the DataItem template</a> example.<br /> When a user types a value, the editor raises the client-side <a href="http://documentation.devexpress.com/#AspNet/DevExpressWebASPxEditorsScriptsASPxClientEdit_ValueChangedtopic"><u>ASPxClientEdit.ValueChanged</u></a> event. In the event handler, it is possible to get a value from the editor and send it to the server using <a href="http://api.jquery.com/jQuery.ajax/"><u>jQuery.ajax</u></a> method.</p>
<p><strong>See Also:<br /> </strong><a href="http://community.devexpress.com/blogs/aspnet/archive/2011/10/06/video-asp-net-mvc-gridview-how-to-setup-multi-row-and-instant-updates.aspx"><u>Video: ASP.NET MVC GridView - How To Setup Multi-Row and Instant Updates</u></a><br /> <a href="https://www.devexpress.com/Support/Center/p/E4073">GridView - How to implement batch update using the Ajax request</a><br /> <a href="https://www.devexpress.com/Support/Center/p/E4236">How to implement the multi-row editing feature in the GridView</a></p>


<h3>Description</h3>

<p>Remove the DevExpress.Web.Linq reference.</p>

<br/>


