Download Link: https://assignmentchef.com/product/solved-csc60-lab-2
<br>
<strong>Lab 2.  UNIX commands.</strong>

<strong><u>Purpose and rationale</u></strong>

The purpose of this lab is to quickly get students up to speed with basic usage of the UNIX development environment, as a preparation for all future lab activities.

<strong><u>Lab environment</u></strong>

All work should be done on a machine in the department’s Linux cluster. Refer to our Lab1 directions. You should use <strong>atoz, sp1, sp2 </strong>or <strong>sp3, instead of athena</strong>.  This is practice for a task later in the semester.

<h1>[<strong>NOTE</strong>: I accessed all four by logging into “athena”, typing “ssh atoz” or “ssh spX”, typing “yes”, and re-entering my password.]</h1>

<strong><u> Part 1. Introductory UNIX lab2 (also known as  <em>Give-Linux-some-time</em>   ):</u></strong>

<ol>

 <li>Read/browse the <strong>man</strong> pages for the Shell commands listed below in #6</li>

 <li>To view the manual for the command “script”, type <strong>man script</strong>.</li>

 <li>Use the space bar to scroll through the display from <strong>man</strong>.</li>

 <li>Type <strong>q</strong> to quit each session.</li>

 <li><strong>SEARCH</strong>. Some of the commands below will show up as CSH_BUILTINS or</li>

</ol>

BASH_BUILTINS

<ol>

 <li>In this mode, the needed information is somewhere in a big display.</li>

 <li>Example: When doing a <strong>man history</strong>, you get more information that you expect.

  <ol>

   <li>Type <strong>/history</strong> to <strong><u>search</u></strong> for the word “history” and see occurrences of that word.</li>

   <li>Typing an <strong>n</strong> will take you to the next occurrence.</li>

  </ol></li>

 <li>Check out the “man” pages for the following two columns of commands.</li>

</ol>

<table width="550">

 <tbody>

  <tr>

   <td width="336">script man (note the standard sections ofthe manual i.e 1, 2, 3 …) who (also try w) gcc  touchtopmkdir   lspscdfile catwcgrep</td>

   <td width="214">cpdiff rm historyjobsmakessh headtaillogoutviview  (<em>This one is buried in the <strong>vi</strong>             page…search for it.) </em>exit</td>

  </tr>

 </tbody>

</table>

<h1> more directions on next page</h1>

<strong><u>Part 2. Prepare a script to show your work:</u></strong>

Run the script command to make a script of your terminal session. At the prompt,     type:  <strong>script StudentName_lab2.txt</strong>

Practice the Shell commands using the below list.

<ul>

 <li>The Part 1 instruction to read/scan the various commands is <strong>not</strong> to be included in your script file.</li>

 <li>At the end of the practice session, please be sure to exit script session with <strong>exit</strong></li>

 <li>If you need to leave the script before you are finished, re-open the script and append to it by typing: <strong>script  –a  txt</strong></li>

 <li>You might run into errors while executing these examples. Look at the errors and see if they make sense. Correct the issues if possible and rerun the commands, and then just keep going.</li>

 <li>Follow the commands as listed below. The occasional extra command (like <strong>ls</strong> , <strong>pwd, </strong>or <strong>cd</strong>, for example) is just fine.</li>

 <li>If you incorrectly type a command, then backspace to fix it, it might look something like this: <strong>[<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="e7858e828b95a79497d6">[email protected]</a> lab2]&gt; wc [K[K[Kgrep lab file1</strong></li>

</ul>

Do not try to edit your script file. Just leave it as is.  I know what it is.

<strong>history -c         C</strong>lear the previous history so your script is not a mile long. <strong>cd csc60 </strong>Move to your directory for this class. <strong>mkdir lab2      </strong>Make a directory named lab2. <strong>cd lab2     </strong>Move to directory lab2.

<table width="577">

 <tbody>

  <tr>

   <td width="95"><strong>pwd</strong></td>

   <td width="482">Print current working directory (lab2).<strong>   </strong>We will be moving back and forth between csc60, lab2,  and aaa.</td>

  </tr>

  <tr>

   <td width="95"><strong>mkdir aaa</strong></td>

   <td width="482">Make a new directory aaa</td>

  </tr>

  <tr>

   <td width="95"><strong>cd aaa</strong></td>

   <td width="482">Change current directory to aaa</td>

  </tr>

  <tr>

   <td width="95"><strong>pwd</strong></td>

   <td width="482">Check that you moved from one directory to another.</td>

  </tr>

  <tr>

   <td width="95"><strong>cd ..</strong></td>

   <td width="482">Change to upper directory</td>

  </tr>

  <tr>

   <td width="95"><strong>pwd</strong></td>

   <td width="482">Print current working directory. You should be back in Lab2</td>

  </tr>

  <tr>

   <td width="95"><strong>ls &gt; file1</strong></td>

   <td width="482">List directory content and redirect output to a file called “file1”</td>

  </tr>

  <tr>

   <td width="95"><strong>cat file1</strong></td>

   <td width="482">Display text content in file1</td>

  </tr>

  <tr>

   <td width="95"><strong>less file1</strong></td>

   <td width="482">Like <em>cat</em> but paginated</td>

  </tr>

  <tr>

   <td width="95"><strong>q</strong></td>

   <td width="482">To quit the <strong>less</strong> command</td>

  </tr>

  <tr>

   <td width="95"><strong>file *</strong></td>

   <td width="482">Check file types of all files</td>

  </tr>

  <tr>

   <td width="95"><strong>wc file1</strong></td>

   <td width="482">Print newline, word, and byte counts for file1</td>

  </tr>

 </tbody>

</table>

<strong>wc *</strong>     Word count all files in directory <strong>grep lab file1</strong>  Find word <em>lab</em> in file1. <strong>cp file1 file2</strong>  Copy file1 to a new file2

<strong>ls          </strong>Check that you have both files <strong>cd aaa           </strong>Move one directory below Lab2.

<strong>cp ../file1 .</strong>       Copy file1 from directory above to here. <em>Note the </em><strong>space-dot</strong><em> at the end of  </em><strong>                </strong><em>             the command.</em>

 <strong>more commands on next page  </strong><strong>  </strong><strong>  </strong>

<strong>ls                     </strong>Check that you got file1 here.

<strong>mv file1 file2</strong>  Rename file1 to file2

<strong>ls                     </strong>Check to see that file 1 changed to file 2

<strong>mv ../file1 .</strong>  Move file1 from directory above to here. <em>Note the </em><strong>space-dot</strong><em> at the end of </em><strong>  </strong><em>the command. </em><strong>cd .</strong>.           Move up to Lab2 <strong>ls     </strong>Check that you now have file2 here.

<strong>cd aaa  </strong>      Move back down to directory aaa <strong>ls         </strong>      Check that aaa still contains both file1 and file2.

<strong>cmp file1 file2</strong>      Compare file1 with file2, show differences. Same file so no <strong>                          </strong>          differences.

<strong>ls &gt; aaalist              </strong>Create a different file

<strong>cmp file1 aaalist    </strong>Now compare two files known to be different <strong>diff file1 aaalist      </strong>Like cmp except shows more info

<strong>rm file1</strong>            Remove file1. Answer the delete prompt with: <strong>y ls   </strong>Verify its removal.

<strong>ps u</strong>                 Show all user’s running Process ID’s

<strong>ps -l</strong>                 Show processes (lower case L) (including Process ID Parent Process ID)

<strong>!! </strong>                    Repeat previous command

<strong>history             </strong>A list of the commands you have done.

<strong>Two</strong> choices here to get from aaa to csc60:

<ul>

 <li><strong>cd .. </strong>Move up a directory to lab2. <strong>                     cd ..           </strong>Move up a directory to csc60.</li>

</ul>

<strong>or do one command instead of the two “cd ..” commands.</strong>

<ul>

 <li><strong>cd ../.. </strong>Move up past lab2 to csc60.</li>

</ul>

<strong>             pwd</strong>     Print current working directory. You should be back in csc60 <strong>cd lab1          </strong>Move down to the lab1 directory

<em>[<strong><u>NOTE 2</u>:</strong> The commands <strong>below</strong> will require that you be on in the directory where <strong>lab1.c</strong> resides.  If you path differs, you still need to move to the directory where your <strong>lab1.c</strong> file resides, and then try these commands.] </em>

<strong>head lab1.c</strong> <em>or</em> <strong>head -20 lab1.c</strong>       List first 10 or 20 lines of code

<strong>q                      </strong>Type q to quite the application

<strong>tail lab1.c</strong> <em>or </em><strong>tail -20 lab1.c</strong>          List last 10 or 20 lines of code

<strong>q                      </strong>Type q to quite the application

<strong>ls -al | less</strong>      Directory listing (too long) ‘piped’ to ‘less’ for viewing

<strong>q                      </strong>Type q to quite the application

<strong>history </strong>           History of commands given

<strong>Quit the script session. <em><u>[Note 3</u>:  </em></strong><em>The script ends when the forked shell exits: (a control-D to exit the <strong>Bourne shell</strong> (sh(1)), and exit; logout or control-d (if ignoreeof is not set) for the <strong>C-shell</strong>, csh(1)).To determine what shell you are in, type:  <strong>echo $SHELL</strong></em>

<strong>exit      </strong>Leave and save the script file. <strong>exit     </strong>Exit your login on sp1, sp2, sp3, or atoz.

<strong><u>Deliverables</u></strong>

Please upload your Lab 2 script file (<strong>StudentName_lab2.txt</strong>) to Canvas.

<strong><u>Note to folks with their own UNIX/Linux machines</u></strong>:

I expect you to do the above assignment.  I expect to see the “history” command.  If you feel it invades your privacy, then you have three choices:

<ul>

 <li>Log off and back in to start a fresh new session;</li>

 <li>At the prompt, type: <strong>history -c</strong>   which will clear the command history of your computer</li>

 <li>Do your work on <em>athena</em> like everyone else.</li>

</ul>

…