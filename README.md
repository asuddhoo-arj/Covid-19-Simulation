# Covid-19-Simulation
A Python code for the graphical simulation of the propagation of and impact of mitigation measures  for Covid-19


# This code simulates the propagation of Covid-19 through a graphical     representation of a sample population with random motion.

## Disclaimer:
### The model used in the code incorporates a number of key assumptions and probabilities which are to be carefully noted. While the purpose of the code is for illustration only, its output should not be used unless specific assistance is sought from experts in the field of epistemology. Any part of the code may be used provided reference is made to the present code.

## The Model:

### Given a random sample of people comprising young people, elderly and those in Care Home, the code uses random motion to simulate the progagation of the disease given an initial number of infected persons. Through close contact, the desease is spread throughout the sample. Detection of infected people can be evoked and those detected sent to Quarantine/Hospital where they have to spend 14 days. Depending on the extent of detection, some infected people will remain in the sample. From hospital, those infected can either recover and go back to the main sample, or be sent to an Intensive Care Unit (ICU), where some may pass away. Those who recovered are assumed to be immuned.
### In addition to testing, the model includes two other features:
### First, the effect on the propagation, of a specified proportion of the sample wearing Personal Protection Equipmemt (PPE), such as face mask; and
### Second, the effect of a specified proportion of the sample practising Social Distancing.
### In each case, the period during which these measures can be specified. In this way easing of a lockdown can be modelled.
### With these features, the efficiency of various measures can be illustrated.

## Input:
### The detailed required inputs are illustrated further below through a built-in GUI. Essentially, the sample size, the composision of the sample in terms of yound and old people, including those residing in Care Homes, the number of people initially infected, the extent of testing available, and the effectiveness of PPE and Social Distancing.

## 'Live' Output:
### The main output is an Animated Graphical Illustration of the random motion of then sample population which also dispalys the propagation of the disease to those who are not infected. The graphical display includes a main area for the randomised motion and also two other designated areas for the Quarantin/Hospital, and ICU respectively. The model persons change colour depending on their status of health.
### A 'live' plot shows the daily rate of infection as well as data pertaining to those who are moved to quarantine and the ICU.

## Convergence:
### Convergence is achieved when there are no new infection for 14 consecutive days and there are no infected persons in the sample. If these conditions are not met, the code should be terminated manually.

## Final Output:
### In the final output, graphical data over the specified number of days regarding the following can be obtained:
###       (i) The cummulative number of infected persons
###       (ii) The cummulative number of persons admitted to Hospital
###       (iii) The cummulative number of people admitted to ICU
###       (iv) The cummulative number of people who recovered
###       (v) The daily number of infected cases
###       (vi) The daily Effective R(zero) (see later)
###       (vii)  the daily number of people who recovered 
###       (viii) The daily number of people admitted to Hospital and ICU

###               and; The daily number of deceased and Total death.


## GUI for Input

![readmeinput](https://user-images.githubusercontent.com/63970623/83265895-0bab8300-a1ba-11ea-96fd-76b4752ca0aa.png)

## Animated Display at different days

![readmeday8](https://user-images.githubusercontent.com/63970623/83266230-75c42800-a1ba-11ea-9898-b76adce29244.png)
![readmeday16](https://user-images.githubusercontent.com/63970623/83266254-7ceb3600-a1ba-11ea-9ce6-f5cd75c5ab5c.png)
![readmeday38](https://user-images.githubusercontent.com/63970623/83266267-81afea00-a1ba-11ea-90b1-0799e918e936.png)
![readmeday77](https://user-images.githubusercontent.com/63970623/83266288-88d6f800-a1ba-11ea-8c4a-074a7da0da88.png)
![readmeday126](https://user-images.githubusercontent.com/63970623/83266299-8d031580-a1ba-11ea-98af-96042bca33d9.png)

## Liveplot
![readmeliveplot](https://user-images.githubusercontent.com/63970623/83266338-98eed780-a1ba-11ea-8c6e-95236a0ea090.png)

## Convergence Plots

### Typical convergence output (may be different due to randomness)

AT CONVERGENCE:

******DAYS TO CONVERGE*******: 123

      :  
People sample Size: 902

Number of Elderly: 180

Number of young: 722

Number in Elderly in Care Home: 9

****:     

Total Number of Infected: 551

Total Number of Non-Infected Young People: 270

Total Number of Non-Infected Elderly People: 77

Total Number of Non-Infected Care Home patients: 4

*****:      

Cummulative Number of people admitted to Qua/Hospital: 546

     Number of Elderly in Qua/Hospital on convergence day: 2
     
     Number of Young in Qua/Hospital on convergence day: 1
     
******:       

Cummulative Number who Recovered: 480

    Number of Young who recovered: 404
    
    Number of Elderly who recovered: 76
    
*******:        

Cummulative Number in ICU patients on convergence day: 68

    Number of Young in ICU: 22
    
    Number of elderly in ICU: 45
    
    Number of Care Home patient in ICU: 1
    
********:        

Total Number of Deaths: 37

### Convergence Plots
![readmesubplots](https://user-images.githubusercontent.com/63970623/83266357-a1471280-a1ba-11ea-8177-bb26bb789b64.png)
![readmedeathplot](https://user-images.githubusercontent.com/63970623/83266372-a73cf380-a1ba-11ea-9efb-e5bbf0061935.png)
