<h2>Cluster Analysis of Bank Marketting Based on Demography, Financial Behavior and Campaign Result</h2>

**Context** </br>
Find the best strategies to improve for the next marketing campaign. How can the financial institution have a greater effectiveness for future marketing campaigns? In order to answer this, we have to analyze the last marketing campaign the bank performed and identify the patterns that will help us find conclusions in order to develop future strategies. </br>
</br>
**Source Data** </br>
https://www.kaggle.com/datasets/janiobachmann/bank-marketing-dataset </br>
[Moro et al., 2014] S. Moro, P. Cortez and P. Rita. A Data-Driven Approach to Predict the Success of Bank Telemarketing. Decision Support Systems, Elsevier, 62:22-31, June 2014

Algorithm = K-Means Clustering </br>
best silhouette score = 0.48245867964416644 </br>
best cluster = 3 </br>

<h3>Result</h3>
<h4>Demograhics</h4>
cluster 1: </br>
- 77% of customers falling under cluster 1 are married and have an average age of 51 years
- Majority have an educational qualification of secondary followed by tertiary then primary.
- The majority job is self employment job. </br>
</br>
cluster 2: </br>
- 51% of customers falling under cluster 2 are married and have an average age of 35 years
- Majority have an educational qualification of secondary followed by tertiary then primary.
- The majority job is blue colar.</br>
</br>
cluster 3: </br>
- 53% of customers falling under cluster 1 are married and have an average age of 39 years
- Majority have an educational qualification of secondary followed by tertiary then primary
- The majority job is self employment job and followed by blue colar

<h4>Financial Behaviour</h4>
cluster 1:</br>

- Average Balance: 2,515.86 (highest)
- Average Default: 0.012 (low, indicating strong financial stability)
- Housing Loan: 41.3% (lowest among all clusters, suggesting fewer customers with mortgages)
- Personal Loan: 14.3% (moderate, indicating low dependence on personal loans)
- Conclusion: Customers in this cluster tend to be wealthier, with high balances and low reliance on housing and personal loans.
</br>
</br>
cluster 2:</br>

- Average Balance: 680.72 (lowest, indicating weaker financial position)
- Average Default: 0.025 (highest, indicating greater default risk)
- Housing Loan: 60.4% (relatively high, suggesting more customers with mortgages)
- Personal Loan: 17.5% (highest, indicating high dependence on personal loans)
- Conclusion: Customers in this cluster may have lower financial stability, with low balances and high reliance on loans.
</br>
</br>
cluster 3: </br>

- Average Balance: 1,315.97 (moderate, between clusters 0 and 1)
- Average Default: 0.008 (lowest, indicating very stable financial situation)
- Housing Loan: 68.4% (highest, suggesting many customers with mortgages)
- Personal Loan: 14.5% (moderate, similar to cluster 0)
- Conclusion: Customers in this cluster likely have moderate financial stability, with decent balances and manageable loan dependency.

  <h4>Campaign Result</h4>
  Cluster 1 </br>
This cluster has the highest average call duration, approximately 291.65 seconds, indicating that customers in this group tend to engage more in conversations. However, the average number of campaign contacts required to reach them is relatively low (2.36), suggesting that while they may take longer to respond, they are easier to reach compared to other clusters. Additionally, the average pdays (5.55) and previous contact count (0.11) indicate that these customers might be newer or less frequently contacted. Most of the previous campaign outcomes for this group are unknown (94.33% po_unknown), with only a small portion being successful (po_success 2.2%). The primary contact method for this cluster is cellular (57.08%), followed by telephone (9.96%) and unknown (32.95%), reflecting a mix of communication approaches.
</br>
</br>
Cluster 2 </br>
This cluster has the shortest average call duration, around 238.22 seconds, indicating potentially less intense or more straightforward interactions. However, it also has the highest average number of campaign contacts (3.22), suggesting a greater effort is required to reach these customers. With a very low pdays value (0.28) and almost zero previous contacts (0.02), this group likely consists of new prospects or customers who have been recently approached. Almost all previous outcomes are unknown (98.40% po_unknown), with a very low success rate (po_success 0.55%). Most contacts in this cluster are made through cellular (61.15%), followed by telephone (4.27%) and unknown (34.58%), indicating a strong preference for mobile communication.
</br>
</br>
Cluster 3 </br>
This cluster has a moderate average call duration (257.37 seconds) but exhibits significantly different characteristics from the other two clusters. It has a very high average pdays (245.21), indicating that these customers are likely older leads who have not been contacted in a long time. Additionally, the number of previous contacts (3.41) is much higher than in the other clusters, suggesting frequent follow-ups. Despite this, the previous campaign success rate is still relatively low (po_success 14.93%), although higher than the other clusters. Most contacts in this group are made via cellular (92.62%), while telephone (6.53%) and unknown (0.85%) make up a much smaller proportion, highlighting a clear preference for mobile communication.
