# Formal Rules for Historical Intuition

To reconstruct 2nd century cultural literature context of Roman satire in Early Christian texts, it is useful to study
what historical intuition is and how it translates to formal rules that can assist in the process of reconstructing history.

### Emotional and spiritual reasoning

A big part of historical intuition is to reflect realistically how people were reasoning emotionally and spiritually.

For example, if there is a text written by a person who is angry,
then it is important to be able to present the text such that people can understand that the person was indeed angry.

However, how do we know when we accurately present something that is vulnerable to human biases?

For example, think about the difference between these situations:

- Anger
- Justified anger

What people mean by "anger" in general, is slightly different from what they mean by "justified anger".
Justified anger has a component of subjectivity that can be problematic for interpretation of texts.

Furthermore, knowing about mental illness, differences in cultures and social upbringing can help to distinguish nuances
in how people are expressing their emotions or are reasoning spiritually.

Due to the complexity of emotional and spiritual reasoning,
it is difficult to come up with fixed formal rules that give reliable reconstruction of history.
This does not mean that it is impossible or unpractical to make an attempt to do so.
There are other areas of science that took long time to achieve, such as meteorology, but was applied successfully.

There is an intuition that people have when reading a text, using their of experience of interpreting emotions and spiritual reasoning
of other people. A combination of using this intuition with formalization, e.g. using logic,
can provide better understanding of how people were thinking in the 2nd century.

### Superstition

People do not have the same set of superstitions through history.
This makes it is sometimes easy to misunderstand how a person is thinking,
because one might interpret what the person is writing as a metaphor,
when the person might have meant it in a more literal way.

In the 2nd century, people regarded spirits as part of what we today consider natural laws.
From the perspective of a person writing a 2nd century text,
that person might have not be considered as particular superstitious at the time.

When a person claims that e.g. an Aeon or angel is an explanation for something, it can be:

1. Attempt to explain a natural phenomena
2. Attempt to attribute spiritual meaning in a superstitious way
3. Both 1) and 2) without carefully separating them

In modern science, we consider 3) mixing explanations of natural phenomena and
to attribute spiritual meaning in a superstitious way as bad practice.
However, in the 2nd century, this kind of mixing was often seen as a sign of prestige.

Using this formal rule, you get a culture in the 2nd century that encourages superstition
while at the same time also encourages attempting to explain natural phenomena.

### A toy model for formal reconstructing of history

To better understand why formal rules are useful in construction of history,
one can use a toy model as a thought experiment:

Suppose that somebody uses [Dyon](https://crates.io/crates/dyon) to organize data about history
and using the features of Dyon to improve the data or detect possible errors.

For example, there could be a list of year intervals `120-130 AD, 140-150 AD`:

```
a := [[120, 130], [140, 150]]
```

In a year interval, the first year should not be greater than the second.
To check that this possible error does not exist in the data, the user can:

1. Check the data manually
2. Write a function that reports any errors of this kind, if they exist in the data

If the user chooses the latter, then one can do this in a few lines of Dyon code:

```
b := any i { a[i][0] > a[i][1] }
if b {println(link {"ERROR: Year interval is wrong\nHere: "str(a[why(b)])})}
```

A such toy model is useful because it illustrates how making formal rules can assist in reconstruction.
If there was an error, then it might be due to human error when inputting the data.
Or, it could be that the sources of the data is wrong or inconsistent.

### Formal rules are useful even when they are not regarded as universally true

In 2nd century texts, one has claims such as:

```
Jesus walked on water.
```

Some people think, due to Christian upbringing or conversion,
that this is an actual event that happened in history.

This means, they disagree with a formal rule that says:

```
No person in history walked on water.
```

Think about why this rule is useful even though it is not universally agreed upon.
If somebody makes this claim by error, such as:

```
Paul walked on water.
```

Then this error can be detected using the rule and corrected.

The claim of walking on water is supposed to be a miracle.
That is the whole point that the author is making.
It is not a miracle if walking on water is a normal event.

However, consider this sentence:

```
Jesus walked to the well.
```

Here, you might think the following rule is absurd:

```
No person in history walked to the well.
```

However, by modifying the rule a bit, it actually reflects a common cultural practice in some places:

```
No man in 1st century walked to the well, if they could make a woman do so instead.
```

There are many exceptions to this rule, but in general,
women went to the well to bring water home, or men to find a bride.
So, when somebody writes about a man walking to the well,
this could be a literary device used to tell the reader that he is looking for someone to marry.

### Example: Zoe is Mary of Magdala in The Gospel of John

In the beginning of The Gospel of John, the author uses "Logos" in the original Greek, which apparently refers to Jesus.
However, people did not have capital letters in the middle of sentences, so another word that might refer to a character
named by a Greek philosophical concept, was "Zoe" (life).
This word was not emphasized later as possible result of human error or political interpretation.

So, who is this Zoe?

There is a woman in The Gospel of John that is more frequently mentioned and put in important situations with Jesus:
Mary of Magdala.

However, in this text, Mary of Magdala does not get an introduction.
We do not know when Jesus meets her for the first time.

Could the text be altered to remove or change when Jesus meets Mary of Magdala?

Yes! When Jesus meets an anonymous Samaritan woman at the well,
this woman could have been originally Mary of Magdala,
since most Early Christians regarded Logos and Zoe as a pair in their mythology.
It was not common for a man to go to the well, because women usually brought water
and men usually only went to the well to find a bride.

Now, this is not conclusive evidence that Mary of Magdala is the consort of Jesus in the original Gospel of John.
Yet, from this reconstruction, one can make a prediction: If an older version of Gospel of John is found,
then it might say that Jesus meets Mary of Magdala at the well.

### Formal rules important for chronology

Here are some formal rules that are important for reconstructing chronology:

1. People get born and die (e.g. not like Melchizedek)
2. People age 1 year per year continuously
3. People do not go into space (e.g. not like Jesus)
4. People do not teleport from one place to another (e.g. not like Philip)
5. People do not ride fantastical animals (e.g. not like Hercules on Pegasus)
6. People do not resurrect themselves or other people (e.g. not like Jesus with Lazarus)
7. People do not time travel

Violations of these rules in stories is a sign that the author is making fantastical claims
that are meant to be miracles and should not in general be regarded as descriptive of actual events.
If people do this to any person, then it is most likely a false claim.

### Grounding historicity in scientific theory

In science, the most accurate theory of history is The Standard Model of Physics.
This theory has been tested more and survived more scientific experiments than any other theory.
It is used to predict phenomena across history ranging from galaxies to nanostructure.

Most physicists regard The Standard Model of Physics only as an effective field theory,
which means that it is making good predictions but is not a complete explanation of all natural phenomena in existence.

The Standard Model of Physics can also make predictions about people,
however, this requires extensive data modelling and simulation on a level that is unpractical today.
Therefore, it is necessary to make formal rules that approximate predictions of The Standard Model of Physics.

Yet, when people disagree about which formal rules to use, one should investigate whether the disagreement
can be solved using The Standard Model of Physics as a benchmark of scientific reliability.
There has been no confirmed evidence until this day about events that conflict with predictions of this theory.
Some scientists claim that The Standard Model of Physics needs to be modified to explain more natural phenomena
that we know exists, but for which we have no reliable data or simpler testable theories.

As a thumb rule, anything that people claim that conflicts with The Standard Model of Physics, is likely false.

For example, two major important features of Early Christian texts that are conflicting with the theory:

1. There is no well defined definition of an Aeon or angel in Early Christian texts
2. There is no well defined definition of miracles in Early Christian texts

Therefore, what Early Christian texts claim about Aeons or angels is suspicious.
It should be treated as a superstitious belief, unless the author emphasizes it as a metaphor.
