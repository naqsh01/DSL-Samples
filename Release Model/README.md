<H1>Application release sample</H1>

<H2>Platform Requirements</H2>
<p>ElectricFlow 6.1

<H2>Instructions</H2>
<ul>
<li>Retrieve these file to a location on the EF server
<li>Edit the "dslDir" in assemble.groovy to point to where this file is located on the EF server
<li>Run the following from the command line on the EF server
```
ectool login <user> <password>
ectool evalDsl --dslFile "assemble.groovy"
ectool runProcedure "On line bank Release" --procedureName "Assemble"
```
<li>Once this procedure has finished executing, you should see the new Release "Quarterly Online Banking Release"
<li>Also created is a procedure to remove all generated objects for this release model, use this to clean up
<ul>