# FTAD - Fine-grained Turn-taking Action Dataset

Dataset for paper "Human-to-Human Conversation Dataset for Learning Fine-grained Turn-taking Action".

## Overview

![pipeline](img/pipeline.png)

![pipeline](img/state.png)

![pipeline](img/sw2001.png)

## Data statistic
 
### Dataset summary

||FTAD-sw|
|---|:--:|
|# of sessions | 2438|
|Avg. session length | 6.33min|
|Avg. session length | 6.33min|
|Word per minute | 201|
|# of Utterances per session | 141.20 |
|# of Utterances per minute | 22.27|
|# of DPs$ per session | 195.32 |
|# of DPs per minute | 30.85|
|# of DPs(w/o Wait) per minute | 13.43|
|Avg. DP alignment error | 420ms |

### Action Distribution
|Action|FTAD-sw|
|---|:--:|
|Grab_Response | 23.7% |
|Grab_Backchannel | 6.1% |
|Grab_Silence | 0.03% |
|Break_Ignore | 3.77% |
|Break_Release | 2.17% |
|Keep | 0.56% |
|Release | 0.88% |
|Grab_Backchannel_Break | 4.71% |
|Grab_Response_Break | 1.34% |
|Wait&Wait_Silence | 56.66% |


## Files
All data files are under FTAD-sw.zip

* `utterrances` contains the strutural annotation of dialogue transcription  
    * `utter.txt`: corpus of dialogue, with each line as an IPU 
    * `decision.txt`: the list of turn-taking decision points and corresponding actions of each dialogue 

* `tasks` contains the turn-taking prediction task data constructed from utterrances
    * `eot.txt`: end of turn prediction
    * `break.txt`: response prediction at opponent's interruption
    * `backchannel.txt`: sequenctial prediction task for backchannel
    * `response_latency.txt`: expected response time prediction



## Data format

