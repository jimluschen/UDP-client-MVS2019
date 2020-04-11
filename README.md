# UDP-client-MVS2019
Web client to read data from an Arduino solar panel monitor circuit

We need a program that can send and retreive data with a roof-mounted circuit that monitors the status of
my solar panel array.  The roof-mounted circuit will be based on an Arduino microcomputer that talks to
several AC power circuit monitors built with the Microchip MCP39F501.

The project will leverage off of an existing UDP Client/Server program someone else wrote 
for the Linux operating system:  https://lettier.github.io/posts/2016-04-26-lets-make-a-ntp-client-in-c.html

	First step: Convert it to run on Microsoft Visual Studio Community 2019 (requires finding equivalent functions
	and libraries, since existing code is not portable and bombs spectacularly in VS2019)

	Second step: Modify to run as a Windows program (current program runs from console)

	Last step:  Modify to provide specific support to get AC power data from Arduino server.

A second software project will be required to build a Web Server into an Arduino that has an Ethernet shield.
