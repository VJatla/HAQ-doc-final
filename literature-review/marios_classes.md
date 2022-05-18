# Marios classes
<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
**Table of Contents**

- [Marios classes](#marios-classes)
    - [CV 2021](#cv-2021)
        - [Multi class classifier Vs multiple binary classifiers](#multi-class-classifier-vs-multiple-binary-classifiers)

<!-- markdown-toc end -->

## CV 2021
### Multi class classifier Vs multiple binary classifiers
*See homeworks from CV 2021 to determine if a combined classifier
that can recognize writing, no-writing, talking and no-talking is
better than one?*

I am documenting *Jason Urvanejo* and *Christine* ECE 516, 2021
homework 3a. He has the following results which is similar to others

| Activity (MultipleFB) | Jason Urvanejo | Christine              |
|-----------------------|----------------|------------------------|
| Talking               | 72             | 66 (reports NaN erros) |
| Writing               | 84             | 93                     |
| Talking + Writing     | 76             | 79                     |

**Inference:** The writing worked better as a binary classifier. Hence
I would like to have a separate binary classifier for typing and
writing.
