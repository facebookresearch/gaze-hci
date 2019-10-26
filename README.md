# gaze-hci

This repository contains a dataset of eye movement data to accompany the following publication: 

Schuetz, I., Murdison, T. S., MacKenzie, K. J., & Zannoli, M. (2019, April). An Explanation of Fitts' Law-like Performance in Gaze-Based Selection Tasks Using a Psychophysics Approach. In Proceedings of the 2019 CHI Conference on Human Factors in Computing Systems (p. 535). ACM. 
[Link to publication on the ACM digital library](https://dl.acm.org/citation.cfm?id=3300765)


## Dataset Structure

- trials.csv: one line per trial
    - participant - randomly assigned participant ID (1-16)
    - trial - trial in order of presentation (1-140)
    - tar_size - target size in degrees
    - sacc_ampl - saccade amplitude in degrees
    - fix_x/y_deg - fixation position in degrees
    - tar_x/y_deg - saccade target position in degrees
    - fix/tar_*_px - same in screen coordinates (pixels)
    - time_* - stimulus timing (eye tracker time stamp, see paper for presentation order)

- p??_gaze.csv
    - time - eye tracker time stamp (ms)
    - xL, yL - screen coordinates for left eye (pixels)
    - xR, yR - screen coordinates for right eye (pixels)

- p??_events.csv
    - start, end - event start and end time (eye tracker time stamp, ms)
    - duration - event duration in ms
    - saccade, blink, fixation - true (1) if line represents corresponding event
    - eye - left (1) or right eye event (2)



## Citing

If you use this dataset, please cite the corresponding publication:

```

@inproceedings{Schuetz:2019:EFL:3290605.3300765,
 author = {Schuetz, Immo and Murdison, T. Scott and MacKenzie, Kevin J. and Zannoli, Marina},
 title = {An Explanation of Fitts' Law-like Performance in Gaze-Based Selection Tasks Using a Psychophysics Approach},
 booktitle = {Proceedings of the 2019 CHI Conference on Human Factors in Computing Systems},
 series = {CHI '19},
 year = {2019},
 isbn = {978-1-4503-5970-2},
 location = {Glasgow, Scotland Uk},
 pages = {535:1--535:13},
 articleno = {535},
 numpages = {13},
 url = {http://doi.acm.org/10.1145/3290605.3300765},
 doi = {10.1145/3290605.3300765},
 acmid = {3300765},
 publisher = {ACM},
 address = {New York, NY, USA},
 keywords = {eye movements, fitts' law, gaze input, gaze selection, saccades, user interfaces},
} 

```

## License
This dataset is MIT licensed, as found in the LICENSE file.