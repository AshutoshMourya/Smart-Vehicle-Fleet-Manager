<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


## Installation

1. Clone the repo
```sh
git clone https://github.com/abhishekpatel946/Smart-Vehicle-Fleet-Manager
```
2. Run
```sh
npm start
```

## Folder Structure
```
├───public                                                                            
└───src 
    ├───assets                                                                            
    └───component                                                                               
        ├───dashboard
        |   └───Dashboard.js
        ├───dashboard_common
        |   └───FooterLayout.js
        |   └───HeaderLayout.js
        ├───firebase
        |   └───FireConfig.js
        ├───Login
        |   └───home.css
        |   └───home.jsx
        └───Logs
            └───Firedata.js
            └───FuelLog.js
            └───FuelRefill.js
            └───MaintainanceLog.js
            └───OverSpeedLog.js
            └───SpeedLog.js
```

### [Issue#10](https://github.com/abhishekpatel946/Smart-Vehicle-Fleet-Manager/issues/10)

In the Smart Vehicle Fleet Manager using Firestore database to store all the data. The problem with how to fetch those data from firestore and represent that data into the logs table.
<br>
In the Dashboard there will be two parts- 1. Charts  2. Log table
<br>
Fetch the recent updated data from firestore and visualize through using this chart.
<br>
And keep all the records in log table and most recently data will be shown in log table to better to readability.

NOTE:- All data on firestore are real-time data which coming from IoT sensors and store on firestore. So be careful with visualization will be real-time up-to-date with data and 
the log table will be maintain to all the record and updated if new data comes in.

### Solution

The data will be store in firestore like this.

![first!](https://github.com/abhishekpatel946/Smart-Vehicle-Fleet-Manager/blob/dashboard/src/assets/1.jpg)

![second!](https://github.com/abhishekpatel946/Smart-Vehicle-Fleet-Manager/blob/dashboard/src/assets/2jpg.jpg)

At this time Firestore database will have only store dummy data for testing.
After code merged successfully then we'll store actual IoT sensors data and visualizing through our charts and maintain logs table for each data record.


### [Issue#12](https://github.com/abhishekpatel946/Smart-Vehicle-Fleet-Manager/issues/12)

Data fetch successfully from firestore but it can't store in SpeedLog pagination table. And also the most recent data display using charts.
<br>
Make sure the all the data record fetch from firestore and keep it in pagination table as a logs history and most recently data used to display using react-fusion charts or widget.
<br>
<br>
Additional if you can improve the performance of fetching data from firestore and rendering it on Dashboard. It will be usefull for us.

### References

- CSS lib
  * [AntDesign](https://ant.design/docs/react/getting-started)
  * [MDBreact](https://mdbootstrap.com/docs/react/getting-started/quick-start/)

- Chart's & Widget
  * [Guage Widget](https://www.fusioncharts.com/charts/gauges/rating-meter-gauge?framework=react)
  * [Bar Chart](https://www.fusioncharts.com/charts/column-bar-charts/simple-column-chart?framework=react)
  * [Line Chart](https://www.fusioncharts.com/charts/line-area-charts/line-chart-with-scrolling-only?framework=react)
  
 - Firebase
   * [Firebase docs](https://firebase.google.com/docs/firestore/quickstart)

### **If you have any better idea to change in database or code too. So feel free to reach me out and tell us! `abhishekpatel946@gmail.com`**
