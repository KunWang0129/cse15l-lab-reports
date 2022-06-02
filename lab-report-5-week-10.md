# This is Kun Wang CSE15L lab report 5

Kun Wang

Professor Soosai Raj

01 June 2022

## Different Tests:
For demonstration purposes, I will use `342.md` and `504.md` as two examples of different output from `my-markdown-parser` and the recent implementation of `markdown-parser`.

I was able to find the tests with different results using `vimdiff` on the result of perspective implementations, here's the picture of the difference:

![342Test](/lab5content/test342.png)

![504Test](/lab5content/test504.png)

Here the link to the test files:

[Link to test 342.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/342.md)

[Link to test 504.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/504.md)

### Test 342.md:
- For test case 342, my implementations gave the correct output as the correct output should be zero links returned

![342Preview](/lab5content/342Preview.png)

![342Test](/lab5content/test342.png)

- My implementation on the left return nothing while the given implementation return a link.
- For test 342, the major fix is regarding the backticks in markdown. Because of the special fuctions of backticks, detections for backticks is needed when running through the “link." 
- A detections of backticks in the `getLinks` or a new method is needed for the fix as it is a minor fix. 
![getLinks](/lab5content/MDGetlink.png)



### Test 504.md:
- For test case 504, neither implementations gave the correct output as correct output should be three links returned: 

![504Preview](/lab5content/504Preview.png)

![504Test](/lab5content/test504.png)

- My implementation on the left returns two link while the given implementation returns nothing.
- A fix for my implementation is in the detection of parenthesis, where different layer of parenthesis in the test caused the missing link. 
- One way to fix the bug is to continue the dectection of `closeParen` until the end of the string. That way can guarentee everything in the link is detected.

![MyFix](/lab5content/MyFix.png)



