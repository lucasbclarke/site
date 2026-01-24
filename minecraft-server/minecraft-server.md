### Minecraft Server

As I was in an elective computing class in highschool, I had the opportunity to bring home an old Dell Inspiron Desktop PC that was at one point used in my school's library, as it had not been used for some time and was of no use to the school.
I opened the PC and cleaned it out with a small hand-blower and a brush to remove the years of dust that had been collecting. Afterwhich I re-pasted the CPU (which was an intel core
2 duo) and re-seeded the ram, however when attempting to power it on it would turn on but not display anything. Despite purchasing a graphics card for the PC (a Nvidia GT210) all I
needed to do was to just insert the ram correctly and then it would have displayed correctly.

The PC remained mostly unused and sat under my table, until one-day where I'd had a flash of inspiration from a video that I had seen online where someone ran their very own Minecraft
server on their own hardware. I installed Ubuntu server onto the PC and downloaded the server.jar from the minecraft website with the requried Java packages to actually run the server
application. The first version that I tried to run was 1.8.9 as I was aware that my CPU was nearly 20 years old, but it did in-fact build and run with no issues. I was able to connect
both from my laptop and from my other gaming PC. Overall, gameplay was quite smooth with only some challenges with chunk rendering when flying in creative mode or another method of 
loading in a large number of chunks.

At the moment I was connecting to my minecraft server directly using the ip address of the Dell server that was running it. However I wanted to be able to connect to the server if I
was using a different internet network, whether I was at school or away from home. So I decided to learn how to forward the port that the server was running on through my home
router so that I would be able to connect to it from any location (as long as the server was on of course). It turned out to be easier than I thought, while just providing the local
ip address that I was currently using to connect and specify the port that would be forwarded. After a short period of time I was able to hotspot my mobile data to my laptop and then
connect through my router's internet ip address and the same port directly to the minecraft server on my home network. As I was in the same room as the server when I conducted this
test I didn't see any noticable performance problems when connecting remotely and everything worked the same as it had on the local network.

Next, I wanted to attempt to run the latest version of minecraft on the server (which at that time was 1.21.10), to see how it would perform. I set it up the same way I had with 1.8.9
by downloading the server.jar file from the minecraft website and then running it on the pc using the java -jar server.jar command. Performance was noticably worse than 1.8.9 as there
was much more to compute for such an old server. However, I was still able to connect through the local and remote networks and play as if it were any other survival server despite
the limitations in performance.

14.12.25 - 08:42 AM AEST
