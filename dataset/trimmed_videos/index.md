# Trimmed videos
<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
**Table of Contents**

- [Trimmed videos](#trimmed-videos)
    - [Old way - Ph.D. proposal](#old-way---phd-proposal)
    - [New way - Ph.D. defense](#new-way---phd-defense)
        - [What is wrong with old way?](#what-is-wrong-with-old-way)

<!-- markdown-toc end -->

Trimmed videos are used to train classifier. The process of creating
them is discussed below.

## Old way - Ph.D. proposal
??? Fill this up later when you have time. For reference the old
documentation can be found at,
- [Group split](./old_way/group_split_old.md)
- [Session split](./old_way/session_split_old.md)

Python code to create these trims are found at the following location,

```
/home/vj/Dropbox/Marios_Shared/HAQ-AOLME/software/HAQ/activity-labels/gt/trims/obsolete/
```

## New way - Ph.D. defense
### What is wrong with old way?
I have found that the trimmed videos created in the [*"Old way"*](#old-way---phd-proposal)
is giving lot of false positives. This is due to,

- **Need more hard samples:** The no-typing and no-writing instances do not provide enough samples
   with hands on the keyboard or paper. This resulted in a classifier
   that classifies every instance with hands on keyboard and paper as
   typing and writing respectively. This led to false positive instances.
- **Training samples should reflect testing:** The samples extracted from the ground truth do not
   reflect in size and shape to the ones created by running detection (keyboard and
   hand detections) framework.
   
### Creating the new dataset 
For creating this new dataset we use,

- **Typing**
  - Keyboard detections
  - Hand detections
  - Typing ground truth
  
- **Writing**
  - Hand detections
  - Writing ground truth
  
[Click here for more details](./new_dataset.md)
