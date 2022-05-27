#### `Installation`

1. Run npm install in both client and server folders
2. After that run npm start in both the folders - Client server will run on localhost:3000 and server runs on localhost:3001
3. Once the app server is up user will be redirected to http://localhost:3000/graphlist where user will see a list of graphs

#### `Technologies/Packages used`
1. Client - React 18, Typescript, Emotion.js with Styled Emotion Components, Jest , Enzyme, Highcharts, HighCharts-react-official, lodash, React error boundry.
2. Server - Node.js, Express.js, uuid, cors.

### `Folder Structure`

Inside src folder - 

components -> A set of reusable components which can be used inside our pages (containers)
conatiners -> Each Component in container represents a Page in 
context -> React context for state management
hooks -> For cutsom hooks
utils -> For Utility functions and types.


#### `Task Completed`

1. Display list of graphs

![image](https://user-images.githubusercontent.com/24535674/170653166-a787ad5a-fe3b-427b-ba9e-c1f499e10ada.png)

2. User has ability to view nodes associated with graph by expanding the accordion

![image](https://user-images.githubusercontent.com/24535674/170653448-300a5315-e5b1-4598-8258-a105fe21bbf3.png)

3. Filter On basis of graphs and nodes - Using loadash debounce for preventing extra re-renders

![image](https://user-images.githubusercontent.com/24535674/170653870-013e4e79-084f-416a-8590-4a011a392507.png)

4. User has the ability to delete graph by clicking on Delete graph button on accordion

5. User can add a new graph with empty nodes and links. Graph name should contain maximum of three charachters long. New graph Id will be created on server side, using uuid module for henerating ids.

![image](https://user-images.githubusercontent.com/24535674/170654431-f9a0304d-4953-4db7-beeb-4c5e5b498c1f.png)

6. Once user clicks on View graph button user is navigated to http://localhost:3000/graph/{graphid} and user can view the graph

![image](https://user-images.githubusercontent.com/24535674/170654911-a079751a-c3a0-44f9-b6cc-792c5687a80e.png)

7. Added unit tests for filter functinality(filter.utils.ts) and App.tsx. 

8. Client is responsive

9. Node labels and links are renderd on each node

10. Add Nodes -> This functianlity is client only and changes will be gone when user refreshes. To add a Node. Click on the node for which u want to add Node and Add Node button should appear as seen in below image.

![image](https://user-images.githubusercontent.com/24535674/170655593-5d9c62b7-ab72-42d4-8868-fb009cc9f36d.png)

Once you click the add Node button, and enter a valid node name node will be added.



