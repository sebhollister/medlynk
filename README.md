# MedLynk -  PPE Supply / Demand Prediction

**Note**: This repository holds the code only for the landing page. The actual code base for the project is still private. Feel free to reach out to seb.hollister@gatech.edu and I'd be happy to talk more about the project. 

![Logo]('pics/logo.jpg')

### MedLynk Project Overview
* Allows hospital supply chain managers to predict their PPE (personal protective equipment) burn rate based on live local data and varying infection rates.
* Additionally, MedLynk provides a framework to not only predict COVID hotspots, but to also intelligently identify clinics that are most vulnerable. 
    * **What Makes a Clinic Vulnerable?**: These clinics we identified were smaller and most likely not part of a large hospital network. Additionally, there were over 20+ types of clinics we identified, ranging from nursing homes to dentists. Since they were not plugged into a PPE supply network, and did not have access to GPOs (group purchasing organizations), these smaller clinics often struggled to secure PPE and fell under the radar. 
    * **Whats the Problem ?**: Within a county/metro area that we predicted would have a COVID spike within 2 weeks, there existed thousands of smaller clinics that fit the identity detailed above. Basically, there was a mismatch of supply. Re-tooled suppliers who shifted to manafacture PPE in order to keep their business alive were outsiders to the PPE game. They didn't have the contacts to get into big hospitals, and didn't have the research ability to identify all these small, at-risk clinics.
    * **How did MedLynk Help?**: MedLynk allowed us to **predict** the metro areas / rural counties that were most likely to see a spike in COVID cases within 2 weeks. Next, we could scrape dozens of public data sources to identify every possible clinic / firm that would need PPE in those counties. Finally, we intelligently filtered the list to identify the clinics that had the most critical need, and would most likely struggle to secure PPE. We compiled this list of thousands of clinics, included contact info and dozens of other data points, and sent the list to retooled suppliers so they could redirect their sales team.
    * **Impact**: We worked with 2 re-tooled suppliers in the Atlanta area who utilized our generated clinic lists to sell their PPE to clinics that they might not have otherwise been aware of. 

### Tools Used
* Web Framework: Flask
* Database: MongoDB (Atlas Cloud implmentation)
* Deep Learning: PyTorch
* Other Python Libraries: Heavily relied on Pandas, Numpy, bs4.
* Custom Javascript, CSS, HTML, Jinja used for frontend. Charts.js for graphs.

### Homepage Screenshot
![Homepage](home_page.PNG)



