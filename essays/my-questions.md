---
layout: essay
type: essay
title: "Smart Questions, Good Answers"
# All dates must be YYYY-MM-DD format!
date: 2024-01-25
published: true
labels:
  - Questions
  - Answers
  - StackOverflow
---

## To Ask, Or Not To Ask

Throughout most of our education, starting from grade school and all through the collegiate level, you hear teachers and professors say things like "Don't be afraid to ask questions!" or "There's no such thing as a dumb/bad/stupid question!" They say these things because questions are important. Asking those who may have more experience on something will most likely lead you to being able to solve whatever problem is in your way. Now, in regards to there being no dumb/bad/stupid questions, this can get a little twisted depending on the what, who, and where you are posing the question. Sure, there may be no such thing as a bad question when dealing with fundamentals or basic concepts, but what about when we come across a broad or complex issue? What if we are encountering errors while trying to setup a virtual machine on our computer? Simply asking the question "How do I configure *this* and *that*" will most likely get you nothing. There is a subtle art to asking questions that is invaluable, especially for those working in technical fields.

Knowing how to ask a "smart" question will most likely get you a "smart" answer.

## Is This A Smart Question?

What makes a question "smart"? What makes a question "not smart"? There are a lot of things that go into what separates the two. Firstly, if the question asked is something that can be answered by doing a simple Google search or looking into a manual or documentation, then it's possible that people may reply along the lines of "STFW" or "RTFM", which help absolutely no one. A good question can usually only be found after you've done a little research into what the problem is or may be. It is also important to include details such as what you were doing/trying to do when the probelm arose, the steps you've taken to try to solve it, the overall goal of what youre trying to accomplish, etc. Being explicit about what exactly you need help on is more likely to attract an experts answer. 

Like I mentioned above, a lot of factors can go into making a "smart" question, so it would be easier to show examples of both a "smart" question and a "not smart" question.

### Stack Overflow: The Good and The Bad

Most of us have heard of Stack Overflow, the question-and-answer site for programmers looking for technical expertise. It is a wonderful resource that should definitely be taken advantage of when you stumble across an issue or just want to see how others handle similar situations. 

Below, I have provided two questions that are pulled from Stack Overflow: the [first question](https://stackoverflow.com/questions/77883544/could-someone-please-explain-how-openai-api-works) is an example of a question that could definietly be improved, and the [second question](https://stackoverflow.com/questions/237104/how-do-i-check-if-an-array-includes-a-value-in-javascript) is one that is more in line with that a "smart" question is.

```
Q. Could someone please explain how Openai api works?

For example I am getting this error:

  raise self._make_status_error_from_response(err.response) from None openai.RateLimitError:
  Error code: 429 - {'error': {'message': 'You exceeded your current quota, please check your
  plan and billing details. For more information on this error, read the docs:
  https://platform.openai.com/docs/guides/error-codes/api-errors.','type':'insuddicient_quota','
  param': None, 'code': 'insufficient_quota'}}

And this is my code:

from openai import OpenAI
client = OpenAI(api_key="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")

response = client.chat.completions.create(
  model="gpt-3.5-turbo",
  messages=[
    {
      "role": "system",
      "content": "Summarize content you are provided with for a second-grade student."
    },
    {
      "role": "user",
      "content": "Jupiter is the fifth planet from the Sun and the largest in the Solar System. It is a gas giant with a mass one-thousandth that of the Sun, but two-and-a-half times that of all the other planets in the Solar System combined. Jupiter is one of the brightest objects visible to the naked eye in the night sky, and has been known to ancient civilizations since before recorded history. It is named after the Roman god Jupiter.[19] When viewed from Earth, Jupiter can be bright enough for its reflected light to cast visible shadows,[20] and is on average the third-brightest natural object in the night sky after the Moon and Venus."
    }
  ],
  temperature=0.7,
  max_tokens=64,
  top_p=1
)

As you can see i am calling gpt-3.5-turbo which is free, also i went online to chatgpt and it is
answering my prompts so why is my code showing 'insufficient_quota'?
```

The above question is asking for help with their code which is supposed to pull an asnwer from gpt-3.5-turbo when given a prompt. The header of the question could definitley be improved. As it is, the header only hints to a limited understanding of the Openai api and doesn't convey that they have a program which needs to be looked at. This could lead to a misunderstanding when people initially click on the question. Another nitpick, no where in the post is there an explicit mention about what kind of specifics are involved: the kind of programming language, the operating system, the IDE that they are using. The last, and perhaps the biggest thing, that makes this question "not smart" is the fact that there is a link to documentation explaining information on the error. Even if they had looked into the documentation, there is no mention of them looking into it, which could lead to redundant replies or even some "STFW" and "RTFM".

```
A. Hopefully that's not your actual secret API key. If it is, you should generate a new one and revoke the old one.

A. From the web page in the error message: Cause: You have run out of credits or hit your maximum monthly spend. Solution: Buy more credits or learn hwo to increase your limits.

A. And the limits are here. If you're using gpt-3.5-turbp, the limit is 3 RPM, 200 RPD. You will need to upgrade to a paid account to increase your limits.

A. gpt-3.5-turbo isn ot free, the API is not the same as the web chatgpt.
```

Shown above are four answers to the question. As we can see, the first answer concerns the potential security issue of posting an API key online, and the next two answers are referencing the link to the error documentation that was posted alongside the error message in the question. The last answer is also referencing something that could be found with a quick Google search into the api. These responses, while helpful, are just referencing things that could be found by either following the error message to the documentation or by looking into gpt-3.5-turbo on the Openapi website. 

Now that we have seen a not so "smart" question, let's take a look at a "smart" question. Below is a question about checking the presence of a value in an array in JavaScript. 

```
Q. How do I check if an array includes a value in JavaScript?

What is the most concise and efficient way to find out if a JavaScript array contains a value?
This is the only way I know to do it:

function contains(a, obj) {
  for (var i = 0; i < a.length; i++) {
    if (a[i] === obj) {
      return true;
    }
  }
  return false;
}

Is there a better and more concise way to accomplish this?

This is very closely related to Stack Overflow question *Best way to find an item in a JavaScript Array?* which addresses finding objects in an array using indexOf.
```

Here, we have a solid and concise header that tells you exactly what they want answers for. Just by looking at the header, we already know that they are working in JavaScript and that they are looking for ways to search an array. We also know that the user already has a working code and is looking for alternative ways to implement it, which is also validated by the fact that they linked another Stack Overflow question regarding the indexOf method. Below are a couple of the posted answers.

```
A. Modern browsers have Array#includes, which does exactly that and is widely supported by everyone except IE:

console.log(['joe','jane','mary'].includes('jane')); //true

You can also use Array#indexOf, which is less direct, but doesn't require polyfills for outdated browsers.

console.log(['joe', 'jane', 'mary'].indexOf('jane') >= 0); // true

Many frameworks also offer similar methods:

* jQuery: $.inArray(value, array, [fromIndex])
* Underscore.js: _.contains(array, value) (also aliased as _.include and _.includes)
* Dojo Toolkit: dojo.indexOf(array, value, [fromIndex, findLast])
* Prototype: array.indexOf(value)
* MooTools: array.indexOf(value)
* MochiKit: findValue(array, value)
* MS Ajax: array.indexOf(value)
* Ext: Ext.Array.contains(array, value)
* Lodash: _.includes(array, value, [from]) (is _.contains prior 4.0.0)
* Ramda: R.includes(value, array)

Notice that some frameworks implement this as a function, while others add the function to the array prototype.
```

This is just one out of 62 possible answers, which show that the question was successful in inciting discussions from a lot of users. There are even updated answers to modernize the post. 

## Conclusion

We all need help throughout our lives. The rate at which the world is evolving and technology is advancing, we need to rely on each other more than ever, and communication is at the heart of it. Knowing how to be efficient and ask "smart" questions is beneficial to everyone involved: the person asking the question gains new insight on how to approach a problem while the people answering get to impart their own knowledge and discuss with others about the topic. 
