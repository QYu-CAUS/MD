<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>test</title>
  <link rel="stylesheet" href="https://stackedit.io/style.css" />
</head>

<body class="stackedit">
  <div class="stackedit__html"><p>**</p>
<h1 id="download-instructions">Download instructions</h1>
<p>**</p>
<ol>
<li>Install Git from “<a href="https://git-scm.com/downloads">https://git-scm.com/downloads</a>”</li>
<li>Get github account from CAUS. send an email to Honghao Tan (<a href="mailto:htan@changanus.com">htan@changanus.com</a>) or Yi Jiang <a href="mailto:yjiang@changanus.com">yjiang@changanus.com</a> to apply for an account.</li>
<li>create an git hub localfolder<br>
For instance,</li>
</ol>
<blockquote>
<p>C:\Users\Work\</p>
</blockquote>
<p>This is TJP SW folder</p>
<ol start="4">
<li>
<p>Download TJP Release SW or development branch to yourTJPFolder<br>
//if you do not see TJP folder ,please send email to   Honghao Tan (<a href="mailto:htan@changanus.com">htan@changanus.com</a>) or Yi Jiang <a href="mailto:yjiang@changanus.com">yjiang@changanus.com</a> ask for access permission//<br>
For instance, in your C:\Users\Work folder</p>
<pre><code>$git clone http://htan@10.80.3.7:7990/scm/cav/tjp.git
</code></pre>
</li>
<li>
<p>Download MIL tool to <a href="http://yourMILfolder.It">yourMILfolder.It</a> is recommended to use the following structure:<br>
In your local github folder C:\Users\Work\ , type in the command</p>
<pre><code>$git clone http://htan@10.80.3.7:7990/scm/cav/digitaltwin.git
</code></pre>
<p>This downloads the master branch by default. It is necessary to swithc to the working branch. For instance, B005. use following command to switch form master to B005 bracnh<br>
$git checkout simB005</p>
</li>
</ol>
<p>Branch convention<br>
MIL tool depends on the SW release version. Therefore, each SW release has its own branch. For instance, simB004 is for B004 SW release/development branch.<br>
SimB005 is for B005 SW release/development branch.</p>
<p>Configure the MIL tool<br>
MIL uses PreScan and Matlab together to run various simulation. open start_Simulation.m in the Branch folder of MIL folder.<br>
For instance, under “C:\Users\Work\digitaltwin\B005_CurveRoad_withRadiusVariable”, find start_Simulation.m. Open it and configure the model library:</p>
<p>For example, the code below links to the B005 development branch.<br>
% release branch of tjp<br>
%cd C:\Users\Work\tjp\010_AdDev\TJP_AutoBoxII<br>
% B005<br>
cd C:\Users\Work\tjp_B005PathCreationBranch\tjp\010_AdDev\TJP_AutoBoxII   // Modifiy this path to your workspace path<br>
% B003<br>
%cd D:\Users\HonghaoTan\GitHub\tjpB003\tjp\010_AdDev\TJP_AutoBoxII</p>
<p>Run simulation<br>
run the start_Simulation.m to load the library and calibration.</p>
<p>FAQ:</p>
<ol>
<li>
<p>Q: when executing start_Simulation.m, matlab gives “ERROR Failed to load library ‘rti1401lib_II_base’ referenced by ‘xyz…abc’”,<br>
A: install the dspace 2017A.</p>
</li>
<li></li>
</ol>
</div>
</body>

</html>
