# Life Time Evanston Performance Dashboard

![Dashboard Preview](https://via.placeholder.com/800x400.png?text=Dashboard+Screenshot)

Interactive prototype for anomaly detection and employee performance analytics at Life Time Evanston.

[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen)](https://roy-torres.github.io/roy-copilot-demo/)

## Features

- **Employee Performance Analytics**
  - Revenue per hour visualization
  - Top/bottom performer identification
  - $15.32 avg revenue/hour tracking
  
- **Personal Training Revenue**
  - Package pricing visualization
  - Signup trend analysis
  - Revenue anomaly detection
  
- **App Engagement Metrics**
  - L•AI•C interaction tracking (+68%)
  - Feature adoption analysis
  - Before/after upgrade comparisons
  
- **AI-Powered Copilot**
  - Performance recommendations
  - Anomaly explanations
  - Actionable insights

## Prototype Walkthrough (Silent Demo)

1. **Employee Performance Tab**
   - Hover over employee bars to see revenue/hour
   - Note color gradient (green → red = high → low performance)
   - Examine Faust's $0/hr (red) vs Lou's $286/hr (green)

2. **Training Revenue Tab**
   - Hover over pricing cards to see details
   - View signup trends in bar chart
   - Note anomaly detection alerts

3. **App Engagement Tab**
   - Compare feature engagement metrics
   - Focus on L•AI•C +68% interaction increase
   - View before/after upgrade charts

4. **Copilot Section**
   - View AI recommendations
   - Click "Apply Recommendations" button
   - Note coaching suggestions for underperformers

## Technical Implementation

```html
<!-- Example Chart Implementation -->
<canvas id="employeeChart"></canvas>

<script>
  // Employee Performance Chart
  new Chart(employeeCtx, {
    type: 'bar',
    data: {
      labels: ['Lou', 'April', 'Jacob', 'Faust'],
      datasets: [{
        label: 'Revenue/Hour',
        data: [286.22, 67.18, 58.61, 0.00],
        backgroundColor: ['#4caf50','#8bc34a','#ffc107','#f44336']
      }]
    }
  });
</script>
