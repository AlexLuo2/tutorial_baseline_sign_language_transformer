# tutorial_baseline_sign_language_transformer
The url of sign language transformer repo is: https://github.com/neccam/slt


## 1.git clone from github repo
1.1 open a terminal and go to the directory where you are going to git clone the repo.

git clone https://github.com/neccam/slt.git xxx(foldername)
 
## 2.set up environment and other required dependencies as the slt repo showed

2.1 put the train and val gzip file into a certain location and configure yaml file.

Be careful about 'tensorflow' and  pytorch related environments. You might need to install those environments that returned error after those not returned errors, manually. (Based on the version you choose to install, you might need to debug the codes as some kind of functions are already depreciated in certain older modules.





 
use pypi website search for the name. (Maybe conda install work as well)

and paste it to your terminal

e.g.

$ pip install xxx==x.x.xx

# 2.2
replace the original train test dev(val) file with the language model you choose to use.
The result is coming from a LLM named I3D. It works on the unwatermarked videos so the acutal result you try it
by yourself may be different from what I get.


2.3 We can use BLEU-1 to BLEU-4, and ROUGE to measure the quality of translation.

tips: You might need to set the the early stop to False in the yaml file to keep the scripts running.
It is recommended to set the number of epoch (training times) to a smaller number. I set it to 100 in my baseline test. 











