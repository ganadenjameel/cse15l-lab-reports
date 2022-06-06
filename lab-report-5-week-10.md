<h1>Using vimdiff on Markdown Parser</h1>

~ Here is the [link](https://github.com/ganadenjameel/markdown-parser) to ***my*** repository <br>
~ Here is the [link](https://github.com/nidhidhamnani/markdown-parser) to ***compared*** repository <br>

## **Test 1**

### Expected Output: [] <br>

![Image](L5SS1.PNG)<br>

[Link](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/402.md) to test file 402<br>

I found this test file by manually scrolling through the vimdiff and looking for differences in the outputs. My implementation for markdown-parser was correct as it did not register any links into the output, unlike the other implementation.

![Image](L5SS3.PNG)<br>

<br>

## **Test 2**

### Expected Output: [] <br>

![Image](L5SS2.PNG)<br>

 [Link](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/409.md) to test file 409<br>

Similar to Test 1, I found this test file by scrolling through the vimdiff and looking for differences in the outputs. My implementation for markdown-parser was incorrect as it registered some form of url when it was not supposed to, while the other implementation worked.

![Image](L5SS4.PNG)<br>