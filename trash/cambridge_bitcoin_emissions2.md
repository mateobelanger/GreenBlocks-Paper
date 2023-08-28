[![Cambridge Centre for Alternative Finance (CCAF.io)](https://firebasestorage.googleapis.com/v0/b/ccaf-afea-test.appspot.com/o/logo.webp?alt=media&token=f4da887e-96cf-4325-b67b-5afd938250bf)](https://ccaf.io/ "CCAF.io")

#### Cambridge Bitcoin Electricity Consumption Index

[Home](https://ccaf.io/ "Home") [About CCAF](https://ccaf.io/about_ccaf "About CCAF") [Contact](https://ccaf.io/contact?topic=cbnsi_btc "Contact")

CBECI

Close

Methodology
===========

Overview  

-----------

### Summary

Following the development of the Cambridge Bitcoin Electricity Consumption Index (CBECI), we wanted to further investigate environmental externalities attributable to the Bitcoin network, more specifically, the impact Bitcoin has on climate change. In recent years, the debate around Bitcoin's sustainability has gained momentum as cryptocurrencies have risen in popularity. So, by adding this new index to the CBECI, we hope to contribute to the debate and offer an approach to quantify the environmental impact.  
  
This issue was looked at from multiple angles and, using similar logic to that behind the CBECI, a sensitivity analysis was performed to identify how greenhouse gas (GHG) emission estimates change as key parameters are altered. Since exact GHG emissions cannot be determined, a hypothetical range consisting of three scenarios is used, two of which form the upper and lower bounds. Within these limits is the best-guess estimate, which represents a more realistic view of Bitcoin's actual GHG emissions.

In this study, the hydro-only scenario (lower bound) is the most environmentally friendly of the three estimates and assumes that all Bitcoin miners use only hydropower. The coal-only scenario (upper bound) is the least environmentally friendly estimate and assumes that all Bitcoin miners use only coal power. The best-guess estimate is based on a more sophisticated approach that leverages additional data on geographical hashrate distribution to differentiate between energy sources used by different countries (or provinces or states) to generate electricity.

 This study's main purpose is to provide a daily annualised (ann.) estimate of the Bitcoin network's GHG emissions. However, due to the lack of data during specific periods, our approach had to be divided into three intervals. These intervals are explained in more detail in later sections. Additionally, our aim to provide daily estimates requires multiple data sources that are continuously updated and available at different frequencies, either on a daily, monthly or yearly basis. This problem is partly addressed by creating clearly defined intervals for periods when no mining map data is available. Another problem is the uneven frequency with which data on electricity mix profiles is reported. Therefore, it was decided to always use the most recently available data for each country, province or state. However, when new data becomes available for a given year, the estimate for the period is adjusted retroactively.1

It is also important to note that this index only considers the environmental impact associated with the electricity consumption of Bitcoin mining and, therefore, cannot be considered a life-cycle assessment. This simplification is based on research conducted by Köhler & Pizzol (2019), who identified geographical distribution and hardware efficiency as the main factors influencing the total environmental footprint, while other factors only had a minor impact (<1%).

### Key terms  

#### Table 1: Introduction to key terms and abbreviations

**Term**

**Explanation**

**(Mt) CO2e**

(Million tonnes) carbon dioxide equivalents

The CO2 equivalent emissions are based on their 100-year global warming potential (GWP100). Other GHGs are converted to an equivalent amount of carbon dioxide.

**ann.**

Annualised

Annual emission estimate based on daily emission estimate. It is assumed that the daily emission value remains constant for 365.25 days.

**Emission intensity**

Life-cycle emissions of electricity generation technologies are given in gCO2e/kWh.

**Electricity mix**

The electricity mix shows the share of the respective primary energy sources in total electricity generation. These include coal, oil, gas, nuclear, hydro, solar, wind and other renewables, as defined in Table 3.

**gCO2e/kWh**

A gram of carbon dioxide equivalent emissions per kilowatt-hour

The measurement of the environmental impact of one kilowatt-hour in carbon dioxide equivalents

**GHG**

Greenhouse gas

Carbon dioxide (CO2), methane (CH4), nitrous oxide (N2O) and fluorinated gases

Model parameters  

-------------------

#### Table 2: GHG index model parameters

**Parameter**

**Description**

**Source**

Estimate of annualised electricity consumption (best guess)

Estimated annualised electricity consumption of the Bitcoin network

Cambridge Centre for Alternative Finance. Available at: [https://demo.ccaf.io/cbeci/index](https://ccaf.io/cbeci/index)

Mining map

Geolocational data of Bitcoin mining operations

Cambridge Centre for Alternative Finance. Available at: [https://demo.ccaf.io/cbeci/mining\_map](https://ccaf.io/cbeci/mining_map)

Life-cycle emission factors for electricity generation technologies

As illustrated in Table 3

National Renewable Energy Laboratory. (2021). _Life Cycle Greenhouse Gas Emissions from Electricity Generation_: _Update._ Golden: NREL

Share of electricity production by source

Determining the most recent electricity mix of all countries for which data is available

Hannah Ritchie and Max Roser (2020). _Energy_ \[online\] OurWorldInData.org. Available at: [https://ourworldindata.org/energy](https://ourworldindata.org/energy)  
  

BP Statistical Review of World Energy. Available at: [https://www.bp.com/en/global/corporate/energy-economics/statistical-review-of-world-energy](https://www.bp.com/en/global/corporate/energy-economics/statistical-review-of-world-energy)  
  

Ember Global Electricity Review (2022). Available at: [https://ember-climate.org/insights/research/global-electricity-review-2022/](https://ember-climate.org/insights/research/global-electricity-review-2022/)  
  

Ember European Electricity Review (2022). Available at: [https://ember-climate.org/project/european-electricity-review-2022/](https://ember-climate.org/project/european-electricity-review-2022/)

Sources of electricity generation by province

A list of the different energy sources used for power generation in Chinese provinces

National Bureau of Statistics. Available at: [http://www.stats.gov.cn/](http://www.stats.gov.cn/)Huajing Industry Research Institute: [https://m.huaon.com/](https://m.huaon.com/)

Sources of electricity generation by state

A list of the different energy sources used for power generation in US states

US Energy Information Administration. Available at: [https://www.eia.gov/electricity/data/state/](https://www.eia.gov/electricity/data/state/)

### Life-cycle greenhouse gas emissions from electricity generation

Table 3 lists the median total life-cycle emission factors (one-time upstream, ongoing combustion, ongoing non-combustion and one-time downstream) for selected electricity generation technologies. The values are based on a systematic review of published life-cycle assessment (LCA) studies conducted by the National Renewable Energy Laboratory (2021).  
  

#### **Table 3: Life-cycle emission factors for electricity generation technologies**

**Electricity generation technology**

**Life-cycle greenhouse gas emissions (gCO2e/kWh)**

Coal

1,001

Oil

840

Gas

486

Nucleara

13

Hydro

21

Solarb

35.5

Windc

13

Other renewablesd

32.3

a Light-water reactor (including pressurised water and boiling water) only, b Mean value of photovoltaic (thin film and crystalline silicon) and concentrating solar power (tower and trough), c Land-based and offshore, d Mean value of geothermal, biomass and ocean.

### Methodology

This section briefly outlines the core concept of our methodology before delving deeper into how the estimates are calculated.

Structurally, this study follows a similar approach to the CBECI by introducing hypothetical lower and upper bounds that form the range of estimated GHG emissions. This is the basis of the sensitivity analysis, which is summarised in Figure 1. The two limits are outlier scenarios based on the abstract assumption that all the electricity used is generated by a single energy source (coal-only or hydro-only). This format is simply illustrative and provides context to make interpreting the results more intuitive. In reality, the electricity used is generated by a mix of energy sources (the electricity mix). Knowing the composition of this mix is essential to computing the emission intensity associated with the Bitcoin network. In this study, the emission intensity serves as a measurement of GHGs emitted per kilowatt-hour, given as gCO2e/kWh. Table 3 lists all the energy sources used in this study with their respective emission intensities.  
  

#### Figure 1: Sensitivity analysis  
  
![](https://firebasestorage.googleapis.com/v0/b/ccaf-afea.appspot.com/o/text_pages%2F3aD3gXUPGtVQs2YU0w7N.png?alt=media&token=cfbcf4f9-43f0-485c-8774-a9fd14d408b6 "Scenario analysis")  

  
While the emission intensity remains constant for both outlier scenarios, as only one energy source powering the Bitcoin network is assumed, the best-guess estimate accounts for all the energy sources in Table 3. This presupposes an understanding of which energy sources are used and to what extent. Therefore, determining the emission intensity of the entire Bitcoin network requires data on the relevant geographical locations of the mining facilities from which the computing power (hashrate) originates and their electricity mix.  
  
Besides showing a range of estimates given different assumptions on the energy sources used, a solution had to be found to deal with periods for which information was unavailable. As mentioned previously, the geographical location of mining facilities is vital to determining the electricity mix. However, data on the geographical distribution of hashrate only started to be collected in September 2019 and is available only until the most recent update of the mining map. Therefore, a solution had to be found for the period before data became available, and for the months for which data was not yet available. To address this challenge, ann. GHG emission estimates are calculated for three different time intervals – **historical**, **assessed** and **predicted** – as shown in Figure 2.  
  

#### Figure 2: Time intervals  
  

![CBECI Mining Map Intervals](https://firebasestorage.googleapis.com/v0/b/ccaf-afea.appspot.com/o/text_pages%2FYOouIuv6f6Eihekzvozy.png?alt=media&token=2d2f8463-edd0-4d0a-aa56-7f06a73551c1 "CBECI Mining Map Intervals")  
  
  
The issue of unavailable data during certain periods only applies to the best-guess estimate, since the upper- and lower-bound estimates are based on a single energy source (coal-only or hydro-only) and, hence, changes in geographical hashrate distribution do not impact the emission intensity. By assuming a single energy source, the emission intensity stays constant over time and always corresponds to the value in Table 3, regardless of where the hashrate originates.  
  
For the best-guess estimate, depending on the time interval, different approaches had to be developed to estimate GHG emissions. The estimates for the **historical** and **predicted** intervals are based on major simplifications, while computing estimates for the **assessed** interval is more complex:

*   The **historical** interval assumes that Bitcoin mining operations are distributed proportionally across the world, based on each country’s share of total global electricity production.
    
*   The **assessed** interval allows for much greater granularity as, during this period, [data](https://ccaf.io/cbeci/mining_map) on global hashrate distribution is available monthly.
    
*   The **predicted** interval assumes that the most recent mining map update is still a valid approximation of the current hashrate distribution.
    

  
The assumptions that underpin each interval have significant implications for the estimated emission intensity during that interval. As illustrated in Figure 3, the emission intensity fluctuates only slightly during the **historical** interval and remains constant during the **predicted** interval. However, when global or regional changes in Bitcoin mining activity are considered, as they are in the **assessed** interval, much greater fluctuations in emission intensity become visible. A more detailed explanation of these assumptions, including the calculations for all our estimates, is provided in the following sections.  
  

#### Figure 3: Emission intensity based on Bitcoin electricity mix  
  

### Upper- and lower-bound estimates

In the upper-bound scenario, it is assumed that all the electricity consumed by Bitcoin miners is generated by coal. In the lower-bound scenario, the assumption is that all the electricity is generated by hydropower. Therefore, the emission intensities of the upper- and lower-bound estimates always equal the emission intensity of the relevant energy source (set _s_), as shown in **Equation 1**.  
  

**Assumption:** The emission intensity of the network (Is,d) is not subject to change and stays constant over time.

  

  
Because it is assumed that a single energy source is used, keeping (_Is,d_) constant, it naturally follows that changes in the geographical locations of mining operations, that would otherwise alter the network's electricity mix profile and thus change the emission intensity, do not influence ann. GHG emissions.

### Best-guess estimate

#### Creating the three intervals

This section describes the three intervals in more detail and the reasoning behind creating them. As mentioned previously, these intervals were created to overcome the issue of data unavailability for certain periods.  
  
First, it is important to highlight a key element that must be considered in the research, namely accounting for the dynamic nature of the Bitcoin mining industry and, specifically, the industry's ability to quickly relocate mining operations within or outside a host country. Being able to account for this dynamic nature is critical, as the location of operations determines the electricity mix profile in the model. Noteworthy are the seasonal migrations within China that demonstrate the importance of this matter, as evidenced in a later section by the severe variations in the country's emission intensity factor during the period for which regional data was available.  
  
Each of the three intervals created – **historical**, **assessed** and **predicted** – uses a different approach to calculating the best-guess estimate. The **historical** interval addresses the unavailability of geolocational data before September 2019 – the first data point provided on our mining map. The **assessed** approach provides the most comprehensive estimate, as geographical hashrate distribution data is available for this interval. However, our most recent mining map data might not represent the current status quo. For example, our most recent mining map data could be as of January 2022, but several months may have passed since that date. This creates a potential gap between the current date and the most recent data available. Since the intention is to provide daily estimates, a new assumption was required to fill this gap, namely that there has been no change in the global hashrate distribution since the last data point in our mining map. This period is the **predicted** interval. However, it is important to note that this interval should be viewed with caution. The reason for this is outlined in more detail in the section on the **predicted** interval.

#### Historical interval

The scope of this study would have been considerably limited if only the period for which data was available was considered. Hence, the **historical** interval was established to account for the absence of mining map data from 18 July 2010 to 31 August 2019, and an alternative approach was created to approximate GHG emissions before 1 September 2019.

**ASSUMPTION:** The **historical** interval is based on the simplified assumption that Bitcoin mining operations are distributed proportionally across the world, based on each country’s share of total global electricity production, implying that the _world electricity mix_ is an accurate approximation.

  
Given the above assumption, the estimated ann. GHG emissions (_Gd_) can be computed using Equations 2 and 3.  
  

and,  

  

#### Assessed interval

The **assessed** interval provides an ann. estimate of GHG emissions for the period between 1 September 2019 and the last day of the month for which mining map data was available. This interval represents the most comprehensive part of our work on Bitcoin's GHG emissions.  
  
While the **historical** interval estimate is based on the simplified assumption that the world electricity mix is an accurate approximation of how the electricity consumed by Bitcoin miners globally is generated, the **assessed** interval accounts for differences in the electricity mix at a country, state or provincial level. This is done by applying a multi-step procedure that segregates countries with a known hashrate into the four categories shown in Table 4.

#### Table 4: Country categories

**Category**

**Countries and jurisdictions**

1

All countries and jurisdictions not mentioned in categories 2–4

2

China

3

The United States

4

The set of countries and jurisdictions listed in Appendix 2

  
  
Segregating countries into different categories is necessary since location-specific peculiarities need to be considered. Category 1 consists of countries (listed in Appendix 1) for which the hashrate distribution is unknown, as opposed to China and the US (categories 2 and 3, respectively), for which more detailed information is available. For countries in category 4 (listed in Appendix 2), either the electricity mix is not available on a country level, or their associated hashrate is likely being inflated.2 The following sections provide a more in-depth description of the four categories.

After calculating the estimated ann. GHG emissions of each country (_Gc,d_) in the four categories, the country GHG emissions are aggregated to form the GHG emissions that can be attributed to Bitcoin (_Gd_), as shown in Equation 4.  
  

  

#### Categories 1 and 4

  
As described below, the associated electricity mix profile is used for countries belonging to category 1, while an alternative approach has been adopted for countries falling under category 4.  
  

**ASSUMPTION:** While _countries in category 1 follow their associated electricity mix profiles_, adjustments had to be made for countries in category 4. _For these countries, the world electricity mix is used as a proxy_ because either no data on the national electricity mix is available or the research team marked them as anomalies. The latter is a corrective measure to address the potential misguidance of miners who deliberately obfuscate their true location by using VPNs or proxy services.

  
Equation 5 shows the calculation of country-specific GHG emissions. Each country's emissions (_Gc,d_) are determined by multiplying the country-specific emission intensity (_Ic,d_) by the country's share of total electricity consumption (_Ec,d_). This approach ensures that regional differences in the emission intensity of power generation and Bitcoin mining activity are considered.  
  

  
While Equation 5 is used for countries in both categories 1 and 4, the equation used for calculating country-specific emission intensities (_Ic,d_) differs.

For each country in category 1, the emission intensity (_Ic,d_) is calculated using the country-specific electricity mix profile. Hence, the value of each country's emission intensity is based on the energy sources used to generate electricity. The share of each energy source (_Sc,s_), derived from the electricity mix of every country, is multiplied by the corresponding emission intensity (_Cs_) of that source. The weighted emission intensities of all sources are then aggregated to form the country's distinct emission intensity (_Ic,d_), as illustrated in Equation 6.  
  

For all countries that fall under category 4, no distinct emission intensities are computed. In this category, country-specific electricity mix profiles are assumed to equal the world electricity mix profile, thus, _Ss,c,d_ = _Ss,d_. Consequently, the emission intensity (_Ic,d_) of all these countries equals the world emission intensity, as shown in Equation 7.  
  

  
Besides examining the differences in country-specific emission intensities, it is also important to distinguish between the scale of Bitcoin mining activity in each country. To accomplish this, the electricity consumption associated with Bitcoin mining in each country (_Ec,d_) must be determined. As illustrated in Equation 8, this value is computed by multiplying each country's share of the total hashrate (_Hc,d_) by Bitcoin's total ann. electricity consumption (_Ed_).  
  

  

#### Category 2

  
The additional information available on geographical hashrate distribution in China allows for a much more granular approach than for countries in categories 1 and 4. Using province-based data was particularly important in capturing seasonal relocations of Bitcoin miners within the country. By relocating from thermal-powered regions to those where hydropower was abundant, opportunistic miners took advantage of favourable electricity rates during the rainy season, when water levels rose. When the dry season arrived and the water levels dropped, miners returned to areas dependent on thermal power. This dynamic within the country consequently significantly altered GHG emissions associated with Bitcoin mining, depending on the season.  
  
On that note, it is important to mention that provincial data is only available for the period between September 2019 and June 2021. Since the government-mandated ban in June 2021 on cryptocurrency mining, no provincial data has been available. However, despite this legislation, Bitcoin mining resumed in China shortly thereafter. Nevertheless, the ban caused miners to seriously consider the trade-offs between maintaining operations and the risk of being discovered.3  
  

**ASSUMPTION 1:** If data on how the hashrate is distributed across provinces in China is not available, but Bitcoin mining activity is detected at a country level, the electricity mix profile of China is used as a proxy. Hence, Equation 5 applies.

Given the logistical steps involved in relocating mining operations and the resulting increased risk of detection, it is assumed that if provincial data is not available, relocations have ceased and, until provincial data is available, any remaining Bitcoin mining activity detected on a country level is evenly distributed across China.  
  
That being said, for the period where provincial data is available, the equation for calculating country-specific GHG emissions (Equation 5) had to be modified to account for this additional data. Equation 9 now follows the same logic as Equation 4 but, rather than aggregating country-level GHG emissions, province-specific GHG emissions are aggregated to determine _GChina,d_, as shown below.  
  

  
Province-specific GHG emissions (_Gp,d_), in turn, are determined by multiplying the emission intensity of each province (_Ip,d_) by the provincial share of China's total electricity consumption (_Ip,d_), as illustrated in Equation 10. This accounts for differences in mining activity between different provinces.  
  

  
Further, differences in the electricity mix of each province also need to be considered. As shown in Equation 11, this was accomplished by multiplying the share of each energy source (_Sp,s,d_), derived from the electricity mix of each province, by the corresponding emission intensity (_Cs_) of that source. The weighted emission intensities of all sources are then aggregated to form a distinct emission intensity for each province (_Ip,d_).  
  

  

Besides examining differences in province-specific emission intensities, it is also important to distinguish between differences in the scale of Bitcoin mining activity across provinces, as this is essential for capturing the impact of the season-based relocations, as shown in Figure 3. This is done by determining the electricity consumption associated with Bitcoin mining for each province (_Ep,d_), as shown in Equation 12.  
  

  
For simplification, it is assumed that China is divided into nine regions: Sichuan, Yunnan, Inner Mongolia, Xinjiang, Beijing, Gansu, Qinghai, Shanxi and 'other provinces'. The electricity mix profiles of all these regions, apart from 'other provinces', correspond to their actual ones. 'Other provinces' is an artificially created region that functions as a proxy for all Chinese provinces other than the eight actual provinces named above. This is a workable simplification as the eight actual provinces account for most of the hashrate. This, however, required the electricity mix and hashrate share for 'other provinces' to be defined as no actual data is available for this region.  
  
  

**ASSUMPTION 2:** China is split into nine regions, each with its own distinct electricity mix profile. Eight of these regions are actual provinces and the ninth represents all other provinces.

  
To isolate the hashrate share of 'other provinces' (_Hp = other provinces_), the sum of hashrate shares of all provinces, where p ≠ 'other provinces',  is deducted from the total, as given by Equation 13.  
  

  
To solve the problem of defining a dedicated electricity profile mix for 'other provinces', the national electricity mix of China was used as a proxy. Thus, the electricity mix profile of 'other provinces' equals that of China’s, as shown in Equation 14.  
  

  

#### Category 3

The data available for the United States also allows for a more granular approach than for countries in categories 1 and 4. With [update v1.2.0](https://ccaf.io/cbeci/change_log) of the CBECI, a regional mining map dedicated to the United States was added to the website, which provides information on hashrate distribution within the country. Knowing each state's share of the overall US hashrate allows Bitcoin mining activity to be matched with the appropriate electricity mix profiles.

**ASSUMPTION 1:** Until data on state-level hashrate distribution becomes available, the country's electricity mix profile is used as a proxy and, thus, the approach outlined in Equation 5 is used for calculating GHG emissions.

**ASSUMPTION 2:** From December 2021, the most recent data available on state-level hashrate distribution is assumed to be the status quo.

  
However, state-level hashrate distribution data is only available from December 2021. Thus, an alternative approach had to be chosen for the period before this more granular dataset became available. Consequently, for the period before December 2021, the same approach used for countries in category 1, shown in Equation 5, was used for the United States. From December 2021, Equation 15 is used.  
  

  
The state-specific GHG emissions (_Gp,d_) are determined by multiplying each state's emission intensity (_Ip,d_) by that state's proportional electricity consumption (_Ep,d_), as illustrated in Equation 16. This accounts for differences in the mining activity and electricity mix in each state.  
  

  
To account for differences in the electricity mix, the share of each energy source (_Sp,s,d_), derived from the electricity mix of each state, is multiplied by the corresponding emission intensity (_Cs_) of that source. The weighted emission intensities of all sources are then aggregated to form the distinct emission intensity of each state (_Ip,d_), as shown in Equation 17.  
  

  
In addition to examining differences in state-specific emissions intensities, it is also important to distinguish between differences in the scale of Bitcoin mining activity across states. This was done by determining the electricity consumption associated with Bitcoin mining in each state (_Ep,d_), as shown in Equation 18.  
  

####   
Predicted interval   
                                                                                

The **predicted** interval was created to find a solution for estimating Bitcoin's ann. GHG emissions daily, even in the absence of mining map data for the period between the most recent data point and the current date in instances where these are not the same, as illustrated in Figure 2. This issue arises because of the different frequencies with which the required data is published, which can lead to an information gap between the latest available data on hashrate distribution and that available on electricity consumption.

**ASSUMPTION:** The most recent mining map data accurately reflects the current geographical hashrate distribution until more recent data becomes available.

While Bitcoin's estimated ann. electricity consumption is published daily, data on geographical hashrate distribution is published infrequently. This means that when calculating the most current estimate of ann. Bitcoin GHG emissions, mining map data is usually unavailable while an estimate on ann. electricity consumption is.  
  
The above assumption solves this problem by assuming the most recent mining map data available is an accurate approximation of the current hashrate distribution. Thus, an estimate of ann. GHG emissions can still be calculated daily, even if the actual hashrate distribution is unknown at that time. This implies that if, for instance, mining map data is available until date _t_, but the current date is _t_1, the geographical hashrate distribution of date _t_ is used as a proxy for the period between the two dates for which data is unavailable.  
  
As shown in Figure 4, after new mining map data has been released, _t_ shifts to the right and represents the month for which the latest data is available. The availability of this new data means the GHG emission estimates of the previously **predicted** interval must be retroactively adjusted and hence become part of the **assessed** interval. Therefore, the data points in the **predicted** interval should be viewed with caution, as they are revised each time the mining map is updated to include data from months that were previously not recorded.

#### Figure 4: The shift from the predicted interval to assessed interval after the release of new mining map data  
  
  

![Time interval](https://firebasestorage.googleapis.com/v0/b/ccaf-afea.appspot.com/o/text_pages%2FBgQhWAQG9wJTFuEepTqC.png?alt=media&token=f2a174d2-a3fc-48fe-8b02-aa2d1bf30c30 "Time interval")

In the **predicted** interval, ann. GHG emissions (_Gd_) are estimated by multiplying the ann. total Bitcoin electricity consumption (_Ed_) by the latest available emission intensity (_It_) in the **assessed** interval, as illustrated in Equation 19.

  
The latest available emission intensity (_It_) is derived by dividing the ann. GHG emission estimate at date _t_ by the ann. total Bitcoin electricity consumption estimate at date _t_, as illustrated in Equation 20. To reiterate, date _t_ represents the last day for which mining map data was available, and, thus, the latest available emission intensity estimate is also at date _t_.  
  

### Limitations of the model

Since our estimate of Bitcoin's GHG emissions is based on previous research on Bitcoin electricity consumption and mining map data, the respective assumptions and limitations of both data sources are also inherited. In addition, a set of new assumptions and limitations have been introduced, specific to determining GHG emissions.  
  
As mentioned in the summary, this study addresses the environmental impact resulting from the use of dedicated mining hardware, i.e., the emissions caused by the electricity consumption required to operate the equipment. (A more detailed explanation of what this comprises can be found on our [website](https://ccaf.io/cbeci/index/methodology).) Therefore, this study cannot be considered a life-cycle assessment. Furthermore, for simplification, we assume that marginal emissions equal average emissions, meaning that the emission intensity (in terms of gCO2e/kWh) of a given location is not influenced by any additional demand created by Bitcoin mining operations. Below is a brief overview of key assumptions carried over from previous studies.  
  
Electricity demand is greatly influenced by electricity rates. For this study, we have used the default [average electricity cost](https://ccaf.io/cbeci/index) per kilowatt-hour, given on our website. Other costs are not considered. Another crucial parameter that determines electricity consumption is the [average efficiency](https://ccaf.io/cbeci/index/methodology) of the mining hardware.  
  
Besides electricity demand, the location of Bitcoin mining operations is of utmost importance. As outlined in the dedicated [methodology](https://ccaf.io/cbeci/mining_map/methodology) section, creating the mining map depends on a sufficiently large sample size and the non-existent or insignificant use of VPNs or proxy services by Bitcoin miners.  
  
In addition to the assumptions and limitations inherited from previous studies, estimating GHG emissions required introducing a new set of assumptions, which include the following:

*   The median GHG emission intensities given in Table 3 represent all countries belonging to one of the four categories listed in Table 4.
    
      
      
    
*   The world electricity mix is a fair approximation if there is no available mining map or country-specific data, or if a country has been flagged as an anomaly (Appendix 2). Because there is ample anecdotal evidence of seasonal relocations of mining operations in China before mining map data was available, we conducted a test to examine how accounting for these relocations would affect cumulative emissions in the **historical** interval. We found that our chosen method (of using the world electricity mix) would slightly overestimate cumulative emissions during this period by 2.96 MtCO2e if these relocations occurred before they were captured in our dataset. A more detailed description of the analysis performed can be found in Appendix 3.  
      
    
*   The most recent update of the mining map is a fair approximation of the current global Bitcoin network hashrate distribution.  
      
    
*   When data is available, it is assumed that the electricity generation mix of a country, province or state is also representative of Bitcoin mining in that region.  
      
    
*   The province-specific electricity generation data of Sichuan, Yunnan, Inner Mongolia, Xinjiang, Beijing, Gansu, Qinghai and Shanxi fairly represents the electricity mix used by Bitcoin miners in each of those provinces. For ‘other provinces’, China's national data is assumed to be a fair representation.  
      
    
*   It is assumed that the amount of electricity demanded by Bitcoin miners remains constant throughout the day and the accessed electricity mix does not vary between daytime and night-time.  
      
    
*   Our estimates do not account for any activities that could reasonably be expected to reduce emissions, such as using flare-gas, off-grid (behind the meter) Bitcoin mining, waste heat recovery or carbon offsetting. Currently, there is little reliable data on these activities, but we are working to incorporate these factors into future versions of the CBECI.
    

 

While most limitations do not have a major impact on the performance of the model, we are aware of its imperfections. The CBECI is an ongoing project that is maintained and refined continuously in response to changing circumstances, with all changes being transparently highlighted in the [Change Log](https://ccaf.io/cbeci/change_log).

If you would like to suggest how we could improve the index, please feel free to send us a [message](https://ccaf.io/contact?topic=cbeci).

### How does our estimate compare to other estimates?

In the past, there have been multiple attempts to analyse Bitcoin's environmental footprint. However, except for the estimate provided by Digiconomist, there is no live index tracking emissions in real time. We would like to point out that emission estimates vary significantly over time, therefore, when comparing emission estimates from different studies, the date of publication should be considered. Moreover, the only GHG considered in some estimates is carbon dioxide (CO2). A non-exhaustive list of available studies and articles is presented in Table 5.  
  