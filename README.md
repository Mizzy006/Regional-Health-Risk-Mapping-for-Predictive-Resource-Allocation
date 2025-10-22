# Regional Health Risk Mapping for Predictive Resource Allocation
Sector: Public Health, Nigeria
Type: Unsupervised Machine Learning, Geospatial Data Analysis
Skills Used: Python (Pandas, Scikit-learn), Cluster Analysis (K-Means), Data Standardization, Data Visualization (Tableau), Policy Recommendation.

## I. Project Goal and Challenge
### The Challenge: Reactive Resource Deployment

Healthcare management in resource-constrained environments often relies on reactive deployment: resources are sent where the outbreak is already severe, leading to high cost, inefficiency, and unequal outcomes. The core problem is the lack of predictive insight into a community’s foundational vulnerability profile.

### The Solution: Predictive Vulnerability Mapping

This project develops a data-driven solution to solve resource misallocation by defining a Community Health Vulnerability Index. We apply Cluster Analysis to segment Local Government Areas (LGAs) into distinct risk profiles, enabling health officials to proactively target scarce resources to the most vulnerable zones.

## II. Methodology and Technical Execution
### Data Strategy

This analysis was based on a synthetic dataset structured on key health determinants found in official Nigerian health surveys, including:
Socioeconomic factors (Poverty Index).
Infrastructure access (Sanitation Deficit Rate, PHC Access Deficit).
Disease Burden (Malaria Prevalence Rate).
Environmental factors (Rainfall Index).

## The Clustering Pipeline
Feature Standardization: All chosen features were standardized to ensure equal weighting in the distance calculation for the clustering algorithm.

Model Selection: K-Means Clustering was selected due to its interpretability and efficiency. The Elbow Method was used to determine the optimal number of clusters, confirming $K=4$ as the best fit for actionable policy segmentation.

Model Execution: The algorithm segmented the LGAs into four distinct groups, allowing for policy differentiation.

## III. Key Results and Actionable Insights

The four clusters identified in the model represent four unique risk profiles. This finding is the basis for a four-tiered resource allocation strategy:

## Critical Risk

Cluster Profile Summary: Low Population Density (Rural), Very High Poverty, Very High Disease Burden, Very Low PHC Access.

Policy Recommendation (Action): MAXIMUM PRIORITY. Immediate deployment of mobile medical teams and emergency supply drops.

## Moderate Risk

Cluster Profile Summary: Moderate Poverty, Moderate Disease Burden, Average PHC Access Deficit.

Policy Recommendation (Action): Sustained Intervention. Focused long-term public health campaigns and infrastructure upgrades.

## Developing Urban, Low Risk
	
Cluster Profile Summary: Near-Average metrics across the board. Stable condition but susceptible to shock.

Policy Recommendation (Action): Preventative Monitoring. Routine surveillance and maintenance of current services.

## Urban Elite,Low Risk

Cluster Profile Summary: High Population Density (Urban/Elite), Very Low Poverty, Excellent Sanitation/PHC Access.

Policy Recommendation (Action): Resource Reallocation. Resources can be safely diverted from these areas to higher-need clusters.

# Visualization (Tableau Output)

The final output is an interactive geospatial dashboard that maps the LGAs and color-codes them according to their assigned Risk Level. 

IV. Conclusion

This project demonstrates the immediate utility of Unsupervised Learning in solving large-scale public health inefficiencies. 
