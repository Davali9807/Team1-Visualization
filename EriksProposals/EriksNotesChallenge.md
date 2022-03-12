# Instructions / goals

* communicate valuable information about the emissions from gas turbine engines around the world.
* o Emissions theme: worst cases, best cases, timeline report, etc.
  o Level of analysis: gas turbine, site, customer, etc.
  o Type of charts: bar, lines, scatter, pie, map, KPIs, gauge, treemap, etc.
  o Functionality of visualizations: interactive, responsive, etc.

* compute the estimated operating hours for a particular gas turbine engine and submit it in this site 
  https://www.bakerhughes.com/gas-turbines/aeroderivative-technology

Evaluation Criteria, the evaluation is divided into
two equal parts: team presentation, and technical approach.

For the Team presentation we will evaluate considering the "Hackathon Rules and Guidelines"
Evaluation Criteria. Keep in mind that the length of the presentation is limited to 30 minutes.
For the Technical approach, we expect you to explore the given data and tell a compelling 
story through the visualizations of your preference, clearly stating the problem or questions that your 
visualizations will help to answer. We will consider:
• Clarity of the analyzed data and its relevance to the proposed problem/question.
• Accuracy of the graphical representation used to convey your message.
• Efficiency of visual effects (use of appropriate shapes, colors and sizes to represent
the analyzed data).
• General evaluation attributes: orthography, originality, authenticity, etc.
• Computational and software resources selected:
• Kaggle score leaderboard (next slide)
• Code submission (with HOURS estimation and visualizations development)
The highest possible score can only be achieved using Python-Kaggle resources. If you
use other languages, you will be given 80% of the points.
For this challenge, along with the presentation you must submit the developed product (report,
dashboard, or a set of visualizations) in pdf format.

## given

* synthetic dataset for the operation of gas turbine engines from different customers sites around the world.

* requesting the submission for scoring of the operating hours estimation (HOURS attribute) for
  -----engine 3 in the ----Ancient Wasp site---- from our ---Busy customer

  * HOURS: operating hours in h.

     This attribute is the accumulated operation time based on the measurements of the ---- compressor speed.
    ---running when: two consecutive measurements of the ---compressor speed > 0
    , then this sampling time is added to the operating hours count.

    The starting value of HOURS for all gas turbine engines is zero.

    Please assume that the gas turbine engines reach a non-zero speed instantly.

    

• site_metadata.csv - geographical information of the sites, and the fuel used at them.
• engine_metadata.csv - information about the gas turbine customers, sites and their corresponding data files.
• dataset.zip - data collected from gas turbine engines as defined in engine_metadata.csv file.
• sample_submission.csv - a sample submission file in the correct format.





### Columns in site_metadata.csv:

• CUSTOMER_NAME: name of customer.
• PLANT_NAME: name of site.
• LATITUDE: in degrees.
• LONGITUDE: in degrees.
• ELEVATION: in meters.
• FUEL_LHV: lower heating value of the fuel in BTU/lb.

### Columns in engine_metadata.csv:

• CUSTOMER_NAME: name of customer.
• PLANT_NAME: name of site.
• ENGINE_ID: engine name.
• FILE_ID: filename with data collected from gas turbine engines.



### Columns in files data_#.csv included in dataset.zip:

• Date: datetime of measurement.
• CMP_SPEED: compressor speed in RPM.      ******** useful
• POWER: power output from the Low-Pressure Turbine (LPT) in 
kW.
• FUEL_FLOW: fuel flow into the combustor in kg/s.
• CO2: carbon dioxide estimated emissions in kg/s.

### Columns in sample_submission.csv:

 • ID: measurement id.
• HOURS: calculated operating hours, h.



A parameter that is usually calculated for gas turbine engines that 
might be useful in your analysis is:
• THRM_EFF: % of thermal efficiency     

![image-20220312065447522](C:\Users\Erik\Documents\BakerHcode\Team1-Visualization\EriksProposals\EriksNotesChallenge.assets\image-20220312065447522.png)



# Will be graded:

Submit your computation of the operating hours estimation for engine 3 in the Ancient Wasp site from our Busy customer, as described in Data.
• Metric to grade
The evaluation metric for the estimation is the Root Mean Square Error (RMSE). As your submission approaches the solution, the Kaggle
score is near to zero.
• Submission Format
Your csv file should contain----- two columns: ID and HOURS. -----

**Where ID** are non-negative integers uniquely identifying the measurements taken from the gas turbine engine,

**and `HOURS`** is your estimation for the operating hours for Busy’s engine 3 at Ancient Wasp, in h.

 A submission example is available at Data. The file must contain a header with the following format:
ID,HOURS
0,0
1,0
2,1
3,2
4,2
…
8760,5498

## submitting

 push the commit of your final code by the same deadline as the Kaggle submission: March 12, 2022 11:00 pm
(CDMX time). Use the form to share the GitHub repository link for the judges to evaluate all deliverables.

https://forms.office.com/r/6qiAqcJHJh

 you must upload the presentation, and
the product (in pdf format) with deadline: March 13, 2022 08:00 am (CDMX time)

 Use the form to share the GitHub repository link for the judges to
evaluate all deliverables.

https://forms.office.com/r/6qiAqcJHJh



 task to deliver a Data
Product about the emissions from gas turbine engines around the world.



