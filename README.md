<div align="center">

## Making Better Variables


</div>

### Description

This article explains proper practices regarding variables, naming them, and choosing the proper variable types for the job.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Peter M\. Dodge](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/peter-m-dodge.md)
**Level**          |Intermediate
**User Rating**    |3.8 (15 globes from 4 users)
**Compatibility**  |VB 5\.0, VB 6\.0
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__1-43.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/peter-m-dodge-making-better-variables__1-40283/archive/master.zip)





### Source Code

<br><br>
<b>Introduction</b><br>
A common question a programmer gets from his (or her) peers is how they can improve upon their coding practices. Along with the commenting practices in my previous article, another way which is quite effective is to use variables in a more proper way.<br><br>
<b>How do I name my variables better?</b><br>
The first step in naming your variables more appropriately is to move from the obscure a's, b's, and x's of infamy to names such as 'tax', 'longestside', and so forth. Descriptively naming your variables makes it much easier to determine what they are used for and this helps the program to withstand maintainance programmer much better, as the maintainance programmer has a much better idea as to what the variable does, especially when descriptive variable names are coupled with the effective commenting practices discussed in my previous article.<br><br>
A pitfall of naming variables is that without a standard system they can fall apart <i>very</i> quickly. That leads to our next section,<br><br>
<b>What naming conventions are commonly used?</b><br>
Most, if not all, variable naming conventions are based upon variable type, and they are usually 1 or 3 letter prefixes attached to the variable name. The LiquidFire standard is a modified version of the Pascal conventions. I provide it as an example below:<br><br>
Single: sng (eg sngPi)<br>
Double: dbl (eg dblPopulation)<br>
Integer: int (eg intAge)<br>
Long: lng (eg lngNumAtoms)<br>
Boolean: bln (eg blnSubDone)<br>
Variant: var (eg varUnknownValue)<br>
String: str (eg strFirstName)<br>
User-Defined type: udt (eg udtPlayerInfo)<br><br>
The common standard has moved more to single letter prefixes (except where the single letter would be duplicated, between the single and string variable types) for convienence, as outlined below:<br><br>
Single: s (eg sPi)<br>
Double: d (eg dPopulation)<br>
Integer: i (eg iAge)<br>
Long: l (eg lNumAtoms)<br>
Boolean: b (eg bSubDone)<br>
Variant: v (eg vUnknownValue)<br>
String: str (eg strFirstName)<br>
User-defined type: u (eg uPlayerInfo)<br><br>
In my experience, the three letter convention makes it easier to determine the type of variable, as it is easier to spot and discern. However, this just comes to preference. Use the system that you prefer, but make sure to use it consistently.<br><br>
<b>What types are appropriate?</b><br>
Choosing the appropriate variable type to implement is an essential programming skill. The appropriate variable choice is highly dependant on the situation.<br><br>
When you have to deal with small numbers without decimals, use an integer. When you need small decimal numbers, then use single.<br><br>
When you need larger numbers, choose a long unless you are absolutely sure these numbers won't include a decimal. Often you can end up with larger numbers with decimals when you don't expect them.<br><br>
For two-state situations such as on/off or yes/no, simply use a boolean variable. The true/false states of this variable type mirrors such situations well.<br><br>
Only use a variant type when you are unsure of what data you are going to have to contain, as variants can take up a good portion of system resources. Variant variables are effective in these situations because they can store any kind of data.<br><br>
When the data is not numerical or boolean (true/false), the only way provided to store it is in a string or variant. In this case, the string variable type is the most efficient way to store data, as it is dynamically resized in memory. This means that whilst the variant type uses as much memory as the largest of the other types, the string variable type uses only as much memory as it needs.<br><br>
<b>Conclusion</b><br>
While there are many ways of improving programming techniques, and a very good step after developing effective commenting practices is to develop your variable usage. Descriptive variable names add to the readability of your code and using effective variable types helps make your program more efficient.<br><br>
<b>Further Reading</b><br>
if you are interested in further improving your programming practices I can recommend both Code Complete by Microsoft Press and my previous article on commenting practices, "Comments: the Good, the Bad, and the Ugly."<br><br>

