Living Documents
===
Some of these features are real and some are yet to be implemented.


Imagine you have an unassuming list.

![Unassuming plain list](https://raw.github.com/samsquire/liveinterface/master/unassuming_list.png "Unassuming plain list")


We can `deconstruct` the list to see the data behind it.

![Deconstructed list](https://raw.github.com/samsquire/liveinterface/master/enrich_list.png "Deconstructed list")


Now imagine you had a more complex list such as a todo list or a list of products as in this example where I am writing a review.

![writing a review?](https://raw.github.com/samsquire/liveinterface/master/live2-a.png "writing a review")

The text in this list is but a small subset of data about the product. In the context of my review, this is the price, my rating and a review. What if you could make the document be aware of your data model?

You are repeatedly asked what something is.

![what is product 1?](https://raw.github.com/samsquire/liveinterface/master/product_1.png "Deconstructed list")

Your answer is used to create the next query.

![what is Product?](https://raw.github.com/samsquire/liveinterface/master/a.png "Deconstructed list")
![what are ratings?](https://raw.github.com/samsquire/liveinterface/master/b.png "Deconstructed list")

Eventually you have a relationship model:

![what is review?](https://raw.github.com/samsquire/liveinterface/master/c.png "Deconstructed list")

When you write your list, you can specify _what_ product you want to refer to as well as the particular fact about that product, such as its rating. 

![writing a review?](https://raw.github.com/samsquire/liveinterface/master/live2-c.png "writing a review")

Now you might want to customize all occurences of a given attribute. Here I can see visualizations of the 'rating'.

![change visualization?](https://raw.github.com/samsquire/liveinterface/master/live2-d.png "change visualization")

Adding magic
===

Our list might not be very useful if we have to hand maintain it all the time. What if we could define a list as the result of a calculation - a bit like a spreadsheet?

So we type some code.

![code recognition](https://raw.github.com/samsquire/liveinterface/master/code-detection.png "code recognition")

The code is recognised by its syntax - red is Ruby and grey is C.

Then it becomes more than just text on a page. It becomes a block of code.

![code block?](https://raw.github.com/samsquire/liveinterface/master/angular-template.png "code block")

This code block could be anything, a Processing script, sourcecode, LATEX or a DSL.

You should be able to interact with the code block. You might execute it or run syntax checkers over it.

Each high level thing on the page has a type and a set of interactions you can carry out with it. The operations and the data for this thing can be provided by another service. This could be a microservice that advertizes its functionality via HAL.

![hal elements](https://raw.github.com/samsquire/liveinterface/master/hateoas.png "hal elements")

Reuse
===

`Semantic autocomplete` gives us a set of options we can use to interact with the document.

![semantic autocomplete](https://raw.github.com/samsquire/liveinterface/master/semantic_autocomplete.png "semantic autocomplete")

`Embed` is to include a thing or a subset of another thing. Here I have three documents. The last document is embedded in the middle and the middle in the first. 

![embed](https://raw.github.com/samsquire/liveinterface/master/embed.png "embed")

We should also be able to transform the thing at this point. Like a spreadsheet, I can define one cell in terms of another. I should be able to click two elements and browse a set of search results for valid transformations involving them.

![graph connection](https://raw.github.com/samsquire/liveinterface/master/graphconnection.png "graph connection")

Shellbucket
===

I can dump output from the terminal into the document for slicing up and reconstruction into something different.

![data bucket](https://raw.github.com/samsquire/liveinterface/master/data_bucket.png "data bucket")

![shellbucket](https://raw.github.com/samsquire/liveinterface/master/shellbucket.png "shell bucket")

![bucket_output](https://raw.github.com/samsquire/liveinterface/master/bucket_output.png "bucket_output")

This would hopefully make creating arbitrary documents possible from different data sources.

