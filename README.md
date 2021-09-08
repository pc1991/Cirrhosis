# Cirrhosis Prediction Dataset 
(Courtesy: fedesoriano of Kaggle)

# Context
Cirrhosis is a late stage of scarring (fibrosis) of the liver caused by many forms of liver diseases and conditions, such as hepatitis and chronic alcoholism. The following data contains the information collected from the Mayo Clinic trial in primary biliary cirrhosis (PBC) of the liver conducted between 1974 and 1984. A description of the clinical background for the trial and the covariates recorded here is in Chapter 0, especially Section 0.2 of Fleming and Harrington, Counting
Processes and Survival Analysis, Wiley, 1991. A more extended discussion can be found in Dickson, et al., Hepatology 10:1-7 (1989) and in Markus, et al., N Eng J of Med 320:1709-13 (1989).

A total of 424 PBC patients, referred to Mayo Clinic during that ten-year interval, met eligibility criteria for the randomized placebo-controlled trial of the drug D-penicillamine. The first 312 cases in the dataset participated in the randomized trial and contain largely complete data. The additional 112 cases did not participate in the clinical trial but consented to have basic measurements recorded and to be followed for survival. Six of those cases were lost to follow-up shortly after diagnosis, so the data here are on an additional 106 cases as well as the 312 randomized participants.

# Attribute Information
1) ID: unique identifier (patient #)
2) N_Days: number of days between registration and the earlier of death, transplantation, or study analysis time in July 1986
3) Status: status of the patient C (censored), CL (censored due to liver tx), or D (death)
4) Drug: type of drug D-penicillamine or placebo
5) Age: age in [days]
6) Sex: M (male) or F (female)
7) Ascites: presence of ascites N (No) or Y (Yes)
8) Hepatomegaly: presence of hepatomegaly N (No) or Y (Yes)
9) Spiders: presence of spiders N (No) or Y (Yes)
10) Edema: presence of edema N (no edema and no diuretic therapy for edema), S (edema present without diuretics, or edema resolved by diuretics), or Y (edema despite diuretic therapy)
11) Bilirubin: serum bilirubin in [mg/dl]
12) Cholesterol: serum cholesterol in [mg/dl]
13) Albumin: albumin in [gm/dl]
14) Copper: urine copper in [ug/day]
15) Alk_Phos: alkaline phosphatase in [U/liter]
16) SGOT: SGOT in [U/ml]
17) Triglycerides: triglicerides in [mg/dl]
18) Platelets: platelets per cubic [ml/1000]
19) Prothrombin: prothrombin time in seconds [s]
20) Stage: histologic stage of disease (1, 2, 3, or 4)

# Correlation Matrix & Scatter Plot of the Relationship b/w N_Days & Alk_Phos

![Correlation Matrix of Relationship between N_Days and Alk_Phos](https://user-images.githubusercontent.com/87962854/132109467-70a01934-9f83-4923-b139-142096294855.png)

![GG Stats Plot of Relationship between N_Days and Alk_Phos](https://user-images.githubusercontent.com/87962854/132109478-d43f118f-9c4d-421b-a011-9a21573b75bb.png)

The above graphs describe how linear the relationship is between the variables. In common sense terms, they simply prove that as the days increase without treatment, the alkaline phosphatase continues to rise causing further liver damage.

# Predictive Relationship b/w the Patient & the Severity of the Patient's Condition

![Predictive Relationship between Patient   Severity of Condition](https://user-images.githubusercontent.com/87962854/132109508-135e0fe1-62c6-44b9-be83-f79fe143c941.png)

Please treat this graph as a map. Take note that the patient number represents the ID of a patient. For each number measures its serious condition. The more serious condition the patient is in, the more vital it is that doctors and nurses must swiftly treat that patient.

# Quantile-Quantile Plot of the Cirrhosis Linear Model

![QQ Plot on the Cirrhosis Linear Model](https://user-images.githubusercontent.com/87962854/132109514-132c377f-a543-440a-a7ca-a73f9778614d.png)

The QQ Plot of this model shows how legitimate this model really is and should be taken seriously.

# Conclusion

Take note that this is data compiled from 1974 to 1984. This survey was published in 1991. There are a lot more technological advances over the years to advance treatment for patients with cirrhosis. However, this data can be used as a tool for doctors, nurses, chemists, and pharmeceutical companies to analyze the deficiencies of these patients and see what potential medications and medical methods can be developed given this information.

# Citations

The dataset can be found in appendix D of:

Fleming, T.R. and Harrington, D.P. (1991) Counting Processes and Survival Analysis. Wiley Series in Probability and Mathematical Statistics: Applied Probability and Statistics, John Wiley and Sons Inc., New York.

Copyright (c) 2021 Robert (Christian) Paul & fedesoriano

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
