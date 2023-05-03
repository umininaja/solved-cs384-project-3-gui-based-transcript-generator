Download Link: https://assignmentchef.com/product/solved-cs384-project-3-gui-based-transcript-generator
<br>
You need to make the transcript for IIT Antartica after generating their results. IIT Antartica since its far away, they were inspired from IIT Logo and replicated it. Refer the tut05 that you have already done, in which you computed SPI CPI. Now the job is to make the SPI CPI output into a PDF for transcript (Check sample transcript: 0402CS99.pdf in transcriptsIITP folder. That needs to be replicated exactly). You can make a gui interface or a web interface. As always use python for processing data but for pdf too you need to use a Python supported pdf generation library (pypdf..etc., there are many).

Options that needs to be provided.

<ol>

 <li>This interface will have option to enter a range of roll numbers. Then on single click the program should generateall the transcript for that range. So if range is 0401cs10-0401cs15, it will generate 6 pdfs. In case the range is 0401cs100401cs80 (and roll number for 0401cs60-0401cs80 dont exists, just dont generate the files for 0401cs60-0401cs80, but do generate the transcript whose roll numbers exists. Also, pop a list saying that these roll numbers dont exists.). A valid range 0401cs60-0401cs60, in this case only one transcript is generated 0401cs60. Save all file names in upper case. When provided a range, do case-insensitive matching. So 0401cs10-0401cs15, 0401cs10-0401CS15, 0401CS10-0401cs15, 0401CS10-0401CS15 generates the same output.</li>

</ol>

Generate all the transcripts in the folder: transcriptsIITP

<ol start="2">

 <li>Option 2 is to generate all transcripts. Here given the grades.csv file, first extract all the unique roll numbers andgenerate all the transcripts in the folder: transcriptsIITP</li>

</ol>

Filename will be <strong>ROLL NUMBER.pdf </strong>in UPPER CASE. If for a student only info till sem4 is available then transcript will be till sem4 only. Page size rule is same, btech a3, others a4.

<strong>Page Size:</strong>

Since BTech is 8 semesters so what happens here you can not fit all the marks on A4 paper so you need to make the PDF size to A3. However for MTech MSc and PhD the semester usually two or four so you can easily fit on A4 sheet so from the roll number check bit 3 and bit 4. That will provide you this information regarding btech, mtech, phd. 01-btech, 11-mtech, 12-msc, 21 phd. if Bit3/bit4 is 01 its btech (so a3 page) and if anything else then assume it to be masters/phd (so A4 page).

Instead of Date of Issue line keep a line for Date Generated, and generate a system date dd-MM-yyyy hh:mm, e.g., 28 Oct 2021, 19:05

<strong>Date Generated: </strong>28 Oct 2021, 19:05. Since this time is system generated, so it will have some offset when computing large number of transcript. So first transcript may have <strong>Date Generated: </strong>28 Oct 2021, 19:05 and the last one may have <strong>Date Generated: </strong>28 Oct 2021, 19:12 depending how many are being generated.

For signature and seal, there should be space provided. In the GUI, keep an option to upload SEAL and signature. Both shall be optional, if not provided, then it will be blank however, the text for signature (Assitant Registrar (Academic)) shall be there irrespctive if sign is there or not.

Helpful links <a href="https://towardsdatascience.com/creating-pdf-files-with-python-ad3ccadfae0f">https://towardsdatascience.com/creating-pdf-files-with-python-ad3ccadfae0f </a><a href="https://stackoverflow.com/questions/2252726/how-to-create-pdf-files-in-python">https://stackoverflow.com/questions/2252726/how-to-create-pdf-files-in-python </a>Check sample transcript: 0402CS99.pdf in transcriptsIITP folder. IITP logo and hindi text is your responsibility to search and add.

1