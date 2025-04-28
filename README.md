# ece46300-lab-1--mac-learning-forwarding-and-stp-solved
**TO GET THIS SOLUTION VISIT:** [ECE46300 Lab 1- MAC Learning, Forwarding, and STP Solved](https://www.ankitcodinghub.com/product/ece46300-lab-1-mac-learning-forwarding-and-stp-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;119778&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ECE46300  Lab 1- MAC Learning, Forwarding, and STP Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
1 Download Lab

Download the Lab 1 files from Brightspace. The source code will be inside the directory “Lab1/”. You must use the environment from Lab 0 to run and test your code. Next, open a terminal and “cd” into the “Lab1/” directory. Now you are ready to run the lab!

2 Task

For this lab, your task is to implement MAC learning, MAC forwarding, and Spanning Tree Protocol (STP). You will create a forwarding table at each switch, and implement STP and MAC learning to populate those forwarding tables. Next, you will implement MAC forwarding at each switch to forward DATA packets using the information in the switch’s forwarding table. For this lab, you can assume that switches and clients never fail. But the link status can change dynamically, i.e., during the runtime, existing links can be removed, or new links can be added, or the link cost can change. Your implementation must be resilient to changes in link status.

3 Source Code

For this lab, you will do your implementation inside a simulated network environment. The simulated network has switches, clients (end hosts), links, and packets just like a real network. Files “switch.py”, “client.py”, “link.py” and “packet.py” contain the implementations of a switch, a client, a link, and a packet respectively. You must not modify any of these files, however you can import the classes defined in these files and use their fields and methods for your implementation. You will do your implementation inside the file “STPswitch.py”. “STPswitch” is a subclass of the “Switch” class and inherits all its fields and methods while overriding its “handlePacket”, “handleNewLink”, “handleRemoveLink”, and “handlePeriodicOps” methods.

“handlePacket” method is called every time a switch receives a packet (DATA or CONTROL).

“handleNewLink” method is called every time a new link (including the initial set of links) is added to the switch or the cost of an existing link changes.

“handleRemoveLink” method is called every time an existing link is removed from the switch.

“handlePeriodicOps” method is called periodically. The period is set using the “heartbeatTime” value in the json file as described in the next section.

You must not override any other “Switch” class methods, but you can add new fields and methods to “STPswitch” as you see fit.

Tip 1: For each switch, all the links directly connected to that switch are stored in the “links” data structure in “switch.py” file. Also, whenever a new link is added or removed or the link cost changes, this information is updated automatically in the “links” data structure and the respective “handle…” method is called.

Tip 2: Go through “packet.py” to understand packet format and types. In particular, there are two kinds of packets – DATA packets that are generated by clients and forwarded by the switches, and CONTROL packets that are generated and exchanged between switches to implement the STP algorithm. Refer to “sendDataPackets” method in “client.py” to understand how new packets are created. Go through “link.py” to understand various link parameters, such as “cost” and “status”.

4 Running the Code

To start the network simulator, run the following command in the terminal,

$ python3 network.py [networkConfigurationFile.json]

The json file argument specifies the configuration of the simulated network. This is explained in the next section. You are provided with three sample json files (“01.json”, “02.json”, “03.json”).

To run the experiments with all the provided network configuration json files, run the following command,

$ ./run_all.sh

To clean temporary files from the previous run of the experiment, run the following command,

$ ./clean.sh

5 Network Configuration Json File

6 Output

At the “endTime”, the simulator cleans up all the active/queued packets in the network, and generates a last batch of broadcast and unicast packets between each pair of clients. It also tracks the route taken by each packet in the last batch, and prints it as the final output on the stdout. For your output to match the correct output, your solution must converge to the correct spanning tree and forwarding table entries before the “endTime”. If the output path between a pair of clients is empty, i.e., [], then it means the packet generated from the source client did not reach the destination client (probably because your solution converged to a wrong route).

7 Grading

We will test your submission against 10 test cases (network configuration json files), for a total of 10 test case runs. For each test case run, if your entire output matches the correct output, you will get 1 point, else a 0. No partial credit. We have provided you with 3 out of those 10 test cases for your testing. The remaining 7 test cases are private, and will not be released at any point. However, we will release your output for each test case run to let you know which test case runs you passed and which ones you failed. You are highly encouraged to create your own test cases to test the robustness of your implementation.

IMPORTANT: Your code must not print any custom / debug statements to the terminal (stdout) other than what the simulator already prints.

Violations of this guideline will result in a 10% grade penalty.

8 Debugging

The provided network configuration json files also contain the correct routes between each pair of clients, which you can use to debug your implementation. Besides, the network simulator also generates .dump files for each switch and client. These files contain information about each packet received by a switch or a client during the runtime of the simulator. A received DATA packet in the dump file will be tagged as “DUP PKT” if the packet is a duplicate of some previously received DATA packet, and tagged as “WRONG DST” if the destination address of the DATA packet does not match the address of the recipient client. You can use these dump files to debug your implementation.

9 A Note About Parallel and Distributed Computation

10 Some Implementation Hints and Guidelines

2. Do not send DATA packets (broadcast or unicast) over the link/port packet arrived on or over an INACTIVE link/port. Ignore any DATA packets received on an INACTIVE link/port.

3. Send CONTROL packets over *all* available links/ports at a switch, including INACTIVE link/port.

4. When Case 2 in STP succeeds, i.e., you choose a new next hop link, make sure to make the new link ACTIVE.

5. After receiving each CONTROL packet, you should check whether the link on which the packet arrived needs to be ACTIVE or INACTIVE, and explicitly change the status of the link as one or the other each time.

6. Remove all entries from the forwarding table corresponding to a link that has become INACTIVE.

11 Submission

You are required to submit a single file “STPswitch.py” on Brightspace.
