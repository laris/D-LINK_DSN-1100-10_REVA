https://arstechnica.com/civis/viewtopic.php?f=16&t=128695
http://linuxmafia.com/faq/Hardware/sata.html#marvell  
(link) Marvell Technology Group Ltd. 88SX7xxx, 88SX6xxx ("Hercules II") and 88SX5xxx/88SX48 ("Hercules I") chip series chips — fakeraid. The 88SX50xx series supports TCQ, but not NCQ or port multipliers. The 88SX60x1 series supports TCQ, NCQ, and port multipliers. libata driver "sata_mv" became available 2005-06 (beta quality as of 2007-02).  

For Marvell chipsets 88SX5040, 88SX5041, 88SX5080, and 88SX5081 "Hercules I" (all SATA-I); and 88SX6041 4-port & 88SX6081 8-port "Hercules II" (both SATA-II), there is a "mvSata" driver from Marvell International Ltd. Like Garzik's libata "sata_mv" driver, Marvell's "mvSata" driver uses the kernel's SCSI layers.  

As of May 2005's v. 3.4.1, that driver changed from proprietary licensing to GPLv2; probably the best revised source code is now Carlos Vidal's file tree, which also has precompiled kernels for Fedora Core and a HOWTO that should generalise well to other distributions. A patch may be necessary to run this driver properly on newer 2.6 kernels.  
Supermicro's ftp site offers proprietary drivers for Marvell 4-port and 8-part SATA chips, written by Adaptec.

https://blog.csdn.net/movno1/article/details/2986285
HighPoint RocketRAID 3520阵列卡的88SX6081-BCZ1控制芯片  
Marvell 88SX6081芯片，是一款采用64-bit 133MHz PCI-X接口的高速8端口磁盘控制芯片，因此主芯片必然要提供PCIe与PCI-X的转接。Marvell 88SX6081支持SATA NCQ以及ATA-6 TCQ，并通过Marvell EDMA引擎减轻CPU的负荷，88SX6081还支持Port Multiplier、SATA Target Mode等高级特性，Marvell 88SX6081采用的64-bit 133MHz PCI-X接口带宽为1.066GB/s，支持8路SATA 3Gbps是足够的。

https://www.marvell.com/company/news/pressDetail.do?releaseID=375

Marvell Introduces the Industry’s First 3 Gbps Serial ATA II Host Controller Solutions for Enterprise Storage Applications
Marvell Extends Serial ATA Leadership Enabling Next Generation Enterprise Storage Features and Performance

Sunnyvale, California (August 18, 2003) –

Marvell® (NASDAQ: MRVL), a technology leader in the development of extreme broadband communications solutions, today announced the industry’s first 3.0 Gbps Serial ATA II PCI-X Host Controllers, enabling the next generation of Enterprise Serial ATA storage applications.  Using the new 88SX6081 (8-port) and 88SX6041 (4-port) Serial ATA II controllers, OEMs are developing the industry’s highest performance, most cost-effective solutions for Server RAID on Motherboard (ROMB), RAID Adapters, Network Attached Storage (NAS), Storage Area Network (SAN), and Nearline Storage Arrays.

Marvell led the industry in adoption of Serial ATA technology with the 2001 introduction of the first Parallel to Serial bridging products and the 2002 introduction of the first 4- and 8-port 88SX50xx PCI-X Serial ATA Host Controllers.  Marvell has shipped over 5 million Serial ATA ports to date and has recorded over 50 design wins with its Serial ATA products.

Serial ATA has enabled a new class of cost-effective primary storage solutions that complements today’s high-end Fibre Channel architectures, when IT budget dollars are at a premium.  The low cost and high capacity of ATA-based Hard Disk Drives (HDD) also provides new options for data backup using Nearline storage to complement traditional Tape Backup systems.

"Serial ATA technology is already becoming a significant force in the development of lower cost server and external disk storage systems, and is ramping in share as the market leaders in these spaces continue to introduce Serial ATA based systems into their product lines", said Sean Lavey, a Semiconductor Analyst with IDC.  "The introduction of Serial ATA II based silicon should accelerate this trend as it provides critical performance improvements necessary for adoption in a wider range of enterprise environments”.

 “We are seeing strong adoption of Serial ATA technology in the market-leading vendors for Servers, RAID Adapters, enterprise RAID Arrays and Nearline storage,” said Balaji Baktha, General Manager of Marvell’s Storage Networking Business Unit.  “Marvell’s Serial ATA II solutions provide these customers a platform to develop a host of next generation enterprise applications.”

The 88SX60xx controllers implement Marvell’s second-generation Serial ATA physical layer (PHY) technology that supports both 1.5 Gbps and 3.0 Gbps operation for high performance Serial ATA backplane implementations.  Spread Spectrum Clocking (SSC) provides optimal EMI performance for lower enclosure costs and easier system certification.

Operation at 3.0 Gbps enables plug-and-play support for next generation Serial ATA II 3.0 Gbps Hard Drives. Serial ATA II Port Multiplier support allows aggregation of multiple 1.5 Gbps Serial ATA links into a single 3.0 Gbps host port for high-density storage enclosures using next generation 2.5” form factor drives.

The 88SX60xx devices implement Serial ATA II Native Command Queuing (NCQ) significantly increasing performance on enterprise applications such as email servers and databases that rely heavily on random accesses.  The 88SX60xx devices also support Serial ATA I/ATA-6 Tag Command Queuing (TCQ) used in Marvell’s first generation 88SX50xx Serial ATA Host Controllers allowing full interoperability with today’s high performance Serial ATA I TCQ drives.

The 88SX60xx software Application Programming Interface (API) compatibility with Marvell’s first generation Serial ATA I Host Controllers enables rapid migration to Serial ATA II technology.  In addition, the API utilizes a SCSI programming model, allowing SCSI applications to be easily ported to Serial ATA HDD subsystems.  Reduced software development cycles offer OEMs using Marvell solutions a significant time to market advantage in a competitive market environment.

About Marvell
Marvell (NASDAQ: MRVL) is the leading global semiconductor provider of complete broadband communications and storage solutions.  The Company’s diverse product portfolio includes switching, transceiver, communications controller, wireless, and storage solutions that power the entire communications infrastructure, including enterprise, metro, home, and storage networking.  As used in this release, the terms “Company” and “Marvell” refer to Marvell Technology Group Ltd. and its subsidiaries, including Marvell Semiconductor, Inc. (MSI), Marvell Asia Pte Ltd. (MAPL), Marvell Japan K.K., Marvell Taiwan Ltd., Marvell International Ltd. (MIL), Marvell U.K. Limited, Marvell Semiconductor Israel Ltd. (MSIL), RADLAN Computer Communications Ltd., and SysKonnect GmbH.  MSI is headquartered in Sunnyvale, Calif., and designs, develops and markets products on behalf of MIL and MAPL.  MSI may be contacted at (408) 222-2500 or at www.marvell.com.

Safe Harbor Statement of Marvell under the Private Securities Litigation Reform Act of 1995:
This release contains forward-looking statements based on projections and assumptions about our products and our markets.  Words such as “anticipates,” “expects,” “intends,” “plans,” “believes,” “seeks,” “estimates,” “may,” “will,” “should,” “continue,” and similar expressions identify forward-looking statements.  Statements that refer to, or are based on projections, uncertain events or assumptions also identify forward-looking statements.  These forward-looking statements are subject to risks and uncertainties, which could cause actual results to differ materially from those discussed in these statements.  Some risks and uncertainties that may cause the statements in this release to differ materially from actual results include, but are not limited to, the timing, cost and successful completion of development and volume production, end-customer qualification and adoption, and the timing, pricing, rescheduling, or cancellation of orders.  For other factors that could cause Marvell’s results to vary from expectations, please see the sections titled “Additional Factors That May Affect Future Results” in Marvell’s annual report on Form 10-K for the year ended February 1, 2003 and Marvell’s subsequent reports on Form 10-Q.  We undertake no obligation to revise or update publicly any forward-looking statements.

Marvell®  and the Marvell logo are trademarks of Marvell.  All other trademarks are the property of their respective owners.
