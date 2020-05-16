# flanker-task

A simple flanker task with three arrows either side of a middle arrow.

To download the whole experiment right click on https://raw.githubusercontent.com/Collector-Trialtypes/flanker-task/master/flanker-experiment.json and click "save link as". Similarly, to save just the trialtype right click on https://raw.githubusercontent.com/Collector-Trialtypes/flanker-task/master/flanker-trialtype.html and click "save link as".

Relevant columns:
- outer_character: the direction of the three arrows on either side of the inner arrow. I've used "<" and ">" characters for the arrows
- inner_character: the direction of the central arrow. I've used "<" and ">" characters for the arrows
- inner_max_time: how long the participant has to response from the presentation of the inner character. If nothing is given then there's no time limit from the presentation of the inner letter.
- correct_response: "left" or "right"
- jitter: the time at the start of the trial before the showing of the outer characters. Either specify a specific time (in ms, but don't write "ms"), or write a range using the following structures:
  - "[minimum jitter] to [maximum jitter]"
  - "[minimum jitter]:[maximum jitter]"
  if nothing is set, there will be 1000ms at the start of the trial before the outer letters are shown.
- inner_wait: the amount of time between the showing of the outer characters and the inner character. Either specify a specific time (in ms, but don't write "ms"), or write a range using the following structures:
  - "[minimum wait] to [maximum wait]"
  - "[minimum wait]:[maximum wait]"
  if nothing is set, there will be 100ms (not 100<ins>**0**</ins>) between showing the inner and outer characters.
- accepted responses: which keyboard characters will be accepted as a response. There's no need for a space or comma between them.
- correct_response: which keyboard character is the correct response for that trial
