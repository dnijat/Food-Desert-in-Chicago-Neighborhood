**Background**

Food access represents a significant urban challenge, particularly within communities lacking
adequate grocery store presence. In Chicago, the concept of food deserts—areas with limited
access to affordable and nutritious food—is increasingly concerning. Several neighborhoods,
particularly those in economically disadvantaged areas, struggle to access fresh produce and
other essential grocery items. This project focuses on identifying these food deserts across
Chicago by analyzing the distribution of and access to grocery stores, aiming to understand the
geographical and socioeconomic factors influencing food availability.

**Methodology**

Our approach focuses on mapping grocery store locations, analyzing their proximity to
neighborhoods, and defining food deserts based on the number of grocery stores available to
residents. By incorporating buffer zones around grocery stores, we ensure a more accurate
representation of accessibility.

**Results**

*Spatial Analysis*

We implemented a 1-mile buffer around each grocery store to effectively assess the extent of
grocery access. This visualization highlights areas served by existing grocery stores and helps prevent the misclassification of neighborhoods as food deserts.
We first calculated the number of grocery stores per 1,000 residents for each area to standardize
access across neighborhoods. Using the 25th percentile (first quartile) of this ratio, we identified
areas with insufficient grocery availability, classifying 19 out of 77 neighborhoods as food
deserts. This threshold ensures focus on areas most underserved
compared to the city-wide average.

The classified food deserts were mapped to visually represent their geographic distribution
across the city. This refined approach not only highlights the areas in dire need of better food
access but also sets the stage for targeted actions to alleviate food scarcity in Chicago’s most
affected neighborhoods.

*Join-count Analysis*

The presence of clustering of food desert neighborhoods was analysed using the join-count
analyses with B (black) for food desert and W (white) for non food desert. In this setting, a BB
join represents the number of a pair of neighborhoods where both are food deserts, WW join
represent the number of a pair of neighborhood where both are non food deserts, and BW join
represents the number of a pair of neighborhood where one location is a food desert and the other
is not. Since the p-value for BB is greater than the conventional significance level 0.05, we
cannot reject the null of spatial randomness in favour of spatial autocorrelation in food deserts. Therefore, we are likely to conclude that food deserts are randomly
located within the Chicago area.

*Regression Analysis*

The correlation displays the overall high number of pairs of variables that are highly correlated. To address the potential multicollinearity problem and make the
model more simple and robust, variance inflation factor (VIF) was employed. Independent variables with corresponding VIF less than 10 were included in the
reduced model.

To determine the model of best fit, R-squared was used as a measure to evaluate the robustness.
As shown in the table, among OLS model, spatial error model, and spatial lag model, spatial lag
model demonstrated highest R-squared, and thus chosen for the further investigation of the
relationship between food desert and the health-/socio- indicators.
Results from the spatial lag regression shows that diabetes_related, a variable indicating the
diabetes-related mortality rate per 100,000 population, is the only variable that is statistically
significantly correlated with food desert (p < 0.05). Also, notice that diabetes_related was not
statistically significant in the OLS model (p = 0.07682). This discrepancy is likely to arise as the
OLS model does not consider the spatial dynamics. Whether a community is a food desert or not
can be highly correlated within a specific region, but by not accounting to spatial features, the
OLS model fails to capture this relationship.
