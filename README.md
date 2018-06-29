# streaming-system-designer
A streaming system designer for apache storm based systems or other streaming systems.

# motivation behind the tool
Often times the best way to understand a streaming system is by watching it
in action.  I created a powerpoint for a system I built in the past to present
to a group of people which worked ok, but during that process
I was thinking it would be interesting to have a little tool to help others
visualize the flow of data in these systems in an easier way.

# pieces of the streaming puzzle for apache storm
- Web Pages (User actions can trigger events to be sent to the server)
- Topologies (We should be able to create topologies or logical groupings of bolts)
- Bolts Within Topologies (Small pieces of code that have one job within a topology,
  can be batched and emit large amounts at once or one at a time)
- External Services (REST services to gather data or any other external service)
- Kafka (Connecting topologies by holding messages for other topologies to read)
- Kafka Connect (A way to move messages from Kafka to HDFS)
- HDFS (Long term storage)

# usage
- Drag and drop all pieces onto system design board
- Hook pieces together
- Define the data for each model as they move from stage to stage
- Define the speed of the data flow for the simulation

# possible programatic usage
- Define operators like in airflow for all pieces
- Be able to connect operators into the structure that you want and have it rendered
  and shown as a simulation