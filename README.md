# Organizational Employee Flow Chart Findings

## What we can do ? (in hack weeks)
- Being able to view in diagram view which employees report to which other employees
- Being able to view in diagram view which employees are part of which departments and their titles
- Being able to view in diagram forms the various departments within an organization
- Being able to see photos of individuals on the org chart
- Being able to reach employee’s profiles and additional details from org chart view
- Some companies may have large numbers of employees/ departments - needs to be designed in a scalable way that will work in this use case
  - Can be done by making chart collapseable and/or zoomable (but data needs to be loaded at once only)

## What we cannot do ? (in hack weeks)
- Hightlight Path for current employees (Comusmes alot of time. There is no easy way to do that i think)
- Basic ability to filter results
- Being able to decide whether or not to use the organization chart feature (if company has bad data for departments or reports to they may wish to disable usage until its cleaned up)
- Being able to view in diagram forms which departments are part of which office (if multiple offices)
- Being able to export the organization diagram to share with other parties (Needs some more research. Maybe it can be done)


## Which libraries can we use ?
1. [D3 Org Charts](https://www.npmjs.com/package/d3-org-chart)
- Highly customized.
- Fulffils most of our requirments.

2. [react-organizational-chart](https://www.npmjs.com/package/react-organizational-chart)
- Can fullfills basic requirments.
- Zoom and collapseable functionality is not supported we nee to add it which is time consuming.

3. We can create it by ourself Which is i think a time consuming task.



In my opinion we can go with D2 org charts as it is a highly customized library and it can fulfill almost all of our requriments.

## Requried things in backend response
- id
- parent id
- other employee details.





### Some more findings 


1. React org charts
 - Advantages 
	 - Basic chart
	 - Supports React Component
- Disadvantages
	 - Needed nested data.
	 - Not expandable or scalable.
 

 2. D3 org chart
 - Advantages
 	- Advance chart.
	- expandable, zoomable
 - Disadvantages
 	- Doesn't support React Component uses plain html as string for node.
 
 
 3. Gojs
 - Advantages
 	- Advance chart.
 	- zoomable
 	- Highly Customizable in sense of ui.

- Disadvantages
	- Needs license
	- Doesn't support React Component as node.
	- not expandable.
	
4. @unicef/react-org-chart
- Advantages
	- Simple Chart
	- Have lazy loading for parent, child and avatar.
	- Have extended and zoom feature.
	- Have image and pdf export feature.

- Disadvantages
	- Not cutomizable in sense of UI.
	- Needed nested data for preloading.
	- Not sure about typescript support
	
	
5. Syncfusion
- Advantage
	- Advance Chart
	- Have zoom feature

- DisAdvantate
	- Doesnot support React component as node.
	- Bit complex to customize ui.
	- Not sure about expandable feature.
