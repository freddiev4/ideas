# Talks

**Intro to Scheduling Algorithms:**
Introduction to scheduling algorithms and their importance, and provide some context.

- Preemptive vs. non-preemptive
- Stateful vs. Stateless

Provide a couple different examples:
- Round Robin
- SJN
  - Minimizes waiting times
  - Requires CPU time to be known
  - Processor should know how much time it takes in advance
- SRT
  - Preemptive version of SJN
  - Often used in batch environments; short jobs need preference
- SCAN (Elevator Algorithm)
- Completely Fair Queuing

**Multithreading & Multiprocessing:**
Introduce the concepts of multithreading & multiprocessing with:

- Conceptual understanding of threads vs processes
- Code examples of both
- Timing of both examples
- Caveats
- What Python does under the hood (CPython)
- Write a blog post on this

Could also split this into two: Threads vs Processes and then a CPython deep-dive

**Using Telemetry to Gather Drone Racing Data in Python/C++:**
Highlight what telemetry is & what sorts of drones use it, and how it can be used
to better monitor your drones and make you better at racing and tuning.

- What is a drone & the parts it's made of
- Different kinds of FCs
- What is telemetry and what FCs support it
- What data can we gather
- How to get that data
- How to store it & analyze it
- What insight we can get from this data
- Python Library?

**Building a Quant Research Group at BU using Quantopian:**
Highlight the problems seen in the discretionary fund and the way students learn within the club, and how
we decided to start a Quant Research arm to educate students about Algorithmic Trading and Quant Finance.

- How we started off
  - Summer Program
  - Many ideas
  - Stuck after running through the lectures
- First Semester
	- First tried to work on the discretionary fund
	- Failed. A lot. Learned from that
- Where we changed focus; Second Semester
  - What roles we decided to add to move the team forward
- Where we're trying to go & potential points of failure/obstacles


**OSS Algo Trading:**
Using [blaze](https://github.com/blaze/blaze), [alphalens](https://github.com/quantopian/alphalens), [zipline](https://github.com/quantopian/zipline), and [pyfolio](https://github.com/quantopian/pyfolio), there could be a talk on how to use all of these open source tools together to:

- Investigate our data
- Come up with a factor that uses that data
- Test it in alphalens
- Use the factor in a long-short equity algorithm
- Run a backtest
- Analyze backtest results


# Projects

**Zipline Bundles Hub:**
A place where people can write code for creating data bundles for various trading calendars and types of data, and then that bundle would be built every night for other users to download.

The APIs that the datasets are built from would have to be public, and users could download the bundles & ingest them by running something like:

`zipline bundle --download <name-of-bundle>` and then `zipline ingest <name-of-bundle>`

**Collision Avoidance for Racing Drones:**
Create a Computer Vision/DL program using [PyTorch](pytorch.org) to create a semi-autonomous drone that is able to do early-collision detection and avoidance. This would be just for fun and would require some sensors for:

- Proximity
- Acceleration (IMU)
- Altitude

And would need a camera for perception. This would probably have to be a brushless motor drone and would need to fall under the micro or 3S classification.
