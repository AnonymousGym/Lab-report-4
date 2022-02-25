# __Lab Report 4__

# 1. The two links to the two repositories.

[Link1][1]

[1]:  https://github.com/sha0xy/markdown-parse


[Link2][2]

[2]:  https://github.com/AnonymousGym/markdown-parse-1

# 2. Show what should be produced.

![Image][111]

[111]: 11.png

![Image][112]

[112]: 12.png

# 3. Show code of MarkdownParseTest.java
This is same for both MarkdownParse.java from two repositories.

![Image][113]

[113]: 13.png

![Image][114]

[114]: 14.png

# 4. Implementation output:
For both my code and the reviewed code, they fail all the tests.

For the first version, the MarkdownParse is below:

![Image][14]

[14]: 4.png

The result is here:

![Image][117]

[117]: 17.png

![Image][118]

[118]: 18.png

For the second version, the MarkdownParse is below:

![Image][16]

[16]: 6.png

The result is here:

![Image][115]

[115]: 15.png

![Image][116]

[116]: 16.png

# 5. Answers to improve the code
  -For backticks: 
  I think there won't be a very easy fix for the problem. The difficulty to identify if a backtick is inside the parenthesis or inside the bracket is hard to be   resolved. From my perspective, we have to check each backtick in the sentence and determine the environment around it. Then, we can judge if it will forbid a     valid link. It will cost a lot of time and space of code.
  
  -For nested parentheses:
  I don't think there is a quick solution for the nested parentheses problem. A typical way to deal with validity of lots of parentheses and brackets is to use a   stack. However, in this case we should keep a structure of []() to keep validity, which needs a more delicately designed stack. So it's hard to finish the       change in 10 lines.
  
  -For new line in parentheses and brackets:
  I believe this is rather difficult for me. Because we have to determine if there is a new line between the two brackets. However, I'm not familiar with the way   to check if there is large space between java code. So, I think it's hard to conquer this problem with a minor improment.
