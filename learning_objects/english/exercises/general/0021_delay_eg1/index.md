---
hruid: g_wacht_vb1
version: 3
language: en
title: "Example Delay 1"
description: "Example Delay 1"
keywords: ["oefeningen", "wacht"]
educational_goals: [
    {source: Source, id: id}, 
    {source: Source2, id: id2}
]
copyright: dwengo
licence: dwengo
content_type: text/markdown
available: true
target_ages: [10, 11, 12]
difficulty: 3
return_value: {
    callback_url: callback-url-example,
    callback_schema: {
        att: test,
        att2: test2
    }
}
content_location: example-location
estimated_time: 5
skos_concepts: [
    'http://ilearn.ilabt.imec.be/vocab/curr1/s-computers-en-systemen'
]
teacher_exclusive: true
---
## Delay

EXERCISE 1

Write a program that does the following:

* Display "Hello people" on the LCD screen for 1 second (1000 ms).
* Display "I am dwenguino" on the LCD screen for 2 seconds (2000 ms).
* Repeat.

Solution:

![blockly](@learning-object/wacht_m1a/en/3)

<div class="alert alert-box alert-success">
The <em>'wait'</em> block that comes <strong>after</strong> a specific instruction, indicates how long the computer must <strong>wait</strong> before starting with the next instruction.
</div>

<div class="alert alert-box alert-danger">
Note that you need to place the code in the <em>'repeat'</em> part of the <em>'setup/repeat'</em> block!<br>
The program only repeats code that is in the <em>'repeat'</em> part.
</div>

***

You will notice that the simulator alternates between "Hello people" and "I am dwenguino". However, this infinite repetition causes a new problem:

![alt](embed/lcdvoorbeeld.png "Example text")

This problem is caused by the fact that the LCD screen does not refresh all characters, but only the ones that change.

> <span style="color:green">H&nbsp;a&nbsp;l&nbsp;&nbsp;l&nbsp;o&nbsp;&nbsp;&nbsp;&nbsp;m&nbsp;e&nbsp;&nbsp;n&nbsp;s&nbsp;e&nbsp;n</span><br>
<span style="color:red">&nbsp;I&nbsp;k&nbsp;&nbsp;&nbsp;&nbsp;b&nbsp;e&nbsp;n&nbsp;&nbsp;&nbsp;&nbsp;D&nbsp;w&nbsp;e&nbsp;n&nbsp;g&nbsp;u&nbsp;i&nbsp;n&nbsp;o</span><br>
<span style="color:green">H&nbsp;a&nbsp;l&nbsp;&nbsp;l&nbsp;o&nbsp;&nbsp;&nbsp;&nbsp;m&nbsp;e&nbsp;&nbsp;n&nbsp;s&nbsp;e&nbsp;n</span><span style="color:red">&nbsp;u&nbsp;i&nbsp;n&nbsp;o</span>

To solve this, use the *'clear LCD screen'-block* to clear the LCD screen each time before new text appears:

![blockly](@learning-object/wacht_m1b/en/3)