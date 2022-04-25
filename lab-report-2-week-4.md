<h1>Bug Fix 1: Empty File</h1>

![Image](EmptyFileErrorFix.PNG)
This is the [file](https://github.com/ganadenjameel/markdown-parser/blob/main/test-file3.md) that caused me to change the code to suit for empty files.<br>


>OUTPUT:<br>
[]

The bug in my code was the inability to check for an **empty** md file and skip it. This bug led to the symptom of an incorrect output as it was supposed to skip the test file entirely. The failure-inducing input was a md file that contained *nothing* within it.



<h1>Bug Fix 2: Missing Open Bracket</h1>

![Image](BracketErrorFix.PNG)
This is the [file](https://github.com/ganadenjameel/markdown-parser/blob/main/test-file2.md) that caused me to edit the code to work with missing open brackets.<br>

> OUTPUT:<br>
Exception in thread "main" java.lang.OutOfMemoryError: Java heap space<br>
at java.base/java.util.Arrays.copyOfRange(Arrays.java:3822)<br>
at java.base/java.lang.StringLatin1.newString(StringLatin1.java:769)<br>
at java.base/java.lang.String.substring(String.java:2709)<br>
at MarkdownParse.getLinks(MarkdownParse.java:19)<br>
at MarkdownParse.main(MarkdownParse.java:30) <br>

The bug in my code was the inability to run through files that had links with missing open square brackets. This bug led to the symptom, an ```OutOfMemoryError```, as the code could not process looking for the **missing** open bracket. The failure-inducing input was a test file that contained a markdown link with an incorrect format; the markdown was missing an open square bracket.



<h1>Bug Fix 3: Images</h1>

![Image](ImageErrorFix.PNG)
This is the [file](https://github.com/ganadenjameel/markdown-parser/blob/main/test-file4.md) that caused me to modify the code to skip images in the code.<br>

>OUTPUT:<br>
[smeltingface.jpg, https://playvalorant.com/en-us/]<br>

The bug in my code was the inability to check for images and continuing to run them through the code as links. This bug led to the symptom of an incorrect output as it returned the image in a link format **"smeltingface.jpg"**. The failure-inducing input was a test file that contained the markdown for an image and a link.
