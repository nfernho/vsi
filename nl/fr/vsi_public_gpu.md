---



copyright:
  years: 2017, 2018
lastupdated: "2018-09-24"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Processeurs graphiques (GPU)
Les processeurs graphiques sont particulièrement adaptés aux charges de travail hautes performances qui nécessitent une plus grande densité de calcul pour réduire la gestion des ressources et les coûts. Ils sont particulièrement adaptés aux processus d'intelligence artificielle, aux applications graphiques et de données intenses, ou au développement de nouvelles applications nécessitant des performances rapides.

Alimentés par les processeurs graphiques NVDIA Tesla, les versions {{site.data.keyword.cloud_notm}} Accelerated Compute “ac1” et "ac2" offrent toutes deux un stockage SSD en bloc et local. Les versions de GPU suivantes sont disponibles :  

  <table>
<CAPTION>Tableau 1. Versions de GPU P100</CAPTION>
<THEAD>
<TR>
<th>Version</th>
<th>GPU</th>
<th>RAM GPU (Go)</th>
<th>UC virtuelle</th>
<th>RAM UC virtuelle (Go)</th>
<th>Type de stockage</th>
<th>Disque d'amorçage (Go)</th>
<th>Disques secondaires (2 et 3) (Go)</th>
</TR>
</THEAD>
<TBODY>
<tr>
<td>ac1.8x60x25</td>
<td>1 P100</td>
<td>16</td>
<td>8</td>
<td>60</td>
<td>En bloc (SAN)</td>
<td>25</td>
<td>Aucun</td>
</tr>
<tr>
<td>ac1.8x60x100</td>
<td>1 P100</td>
<td>16</td>
<td>8</td>
<td>60</td>
<td>SSD local ou SAN</td>
<td>100</td>
<td>Aucun (SAN)<br>300 (local)</td>
</tr>
<tr>
<td>ac1.16x120x25</td>
<td>2 P100</td>
<td>32</td>
<td>16</td>
<td>120</td>
<td>En bloc (SAN)</td>
<td>25</td>
<td>Aucun</td>
</tr>
<tr>
<td>ac1.16x120x100</td>
<td>2 P100</td>
<td>32</td>
<td>16</td>
<td>120</td>
<td>SSD local ou SAN</td>
<td>100</td>
<td>Aucun (SAN)<br>600 (local)</td></tr>

</TBODY>
</table>

**Remarque :** les versions de GPU P100 sont disponibles dans les centres de données _DAL13_, _LON06_ et _WDC07_.

<table>
<CAPTION>Tableau 2. Versions de GPU V100</CAPTION>
<THEAD>
<TR>
<th>Version</th>
<th>GPU</th>
<th>RAM GPU (Go)</th>
<th>UC virtuelle</th>
<th>RAM UC virtuelle (Go)</th>
<th>Type de stockage</th>
<th>Disque d'amorçage (Go)</th>
<th>Disques secondaires (2 et 3) (Go)</th>
</TR>
</THEAD>
<TBODY>
<tr>
<td>ac2.8x60x25</td>
<td>1 V100</td>
<td>16</td>
<td>8</td>
<td>60</td>
<td>En bloc (SAN)</td>
<td>25</td>
<td>Aucun</td>
</tr>
<tr>
<td>ac2.8x60x100</td>
<td>1 V100</td>
<td>16</td>
<td>8</td>
<td>60</td>
<td>SSD local ou SAN</td>
<td>100</td>
<td>Aucun (SAN)<br>300 (local)</td>
</tr>
<tr>
<td>ac2.16x120x25</td>
<td>2 V100</td>
<td>32</td>
<td>16</td>
<td>120</td>
<td>En bloc (SAN)</td>
<td>25</td>
<td>Aucun</td>
</tr>
<tr>
<td>ac2.16x120x100</td>
<td>2 V100</td>
<td>32</td>
<td>16</td>
<td>120</td>
<td>SSD local ou SAN</td>
<td>100</td>
<td>Aucun (SAN)<br>600 (local)</td></tr>

</TBODY>
</table>

**Remarque :** les versions de GPU V100 sont disponibles dans les centres de données _DAL10_, _DAL12_ et _LON04_<!--WDC07-->.


## Avant de commencer
Vérifiez les conditions requises ci-dessous pour le GPU.

1. Les serveurs virtuels de version de GPU sont uniquement disponibles sur un système d'exploitation prenant en charge le mode d'amorçage HVM (Hardware Virtual Machine). Consultez la liste suivante pour connaître les systèmes d'exploitation prenant en charge le mode d'amorçage HVM.  
  - CentOS 7
  - Debian 8
  - RHEL 7
  - Ubuntu 16
  - Windows 2012 R2
  - Windows 2016

2. Des pilotes NVIDIA et des logiciels appropriés doivent être installés. Pour en savoir plus sur les logiciels et les pilotes NVIDIA, voir [Installation de pilotes de GPU et de progiciels](../vsi/vsi_gpu_nvidia_drivers.html).  
**Remarque :** le logiciel que vous installez peut nécessiter des conditions logicielles particulières ainsi que des configurations spécifiques au système d'exploitation.

## Ajout ou suppression de processus graphiques 
Vous pouvez changer le nombre de processeurs graphiques sur votre serveur virtuel après votre commande initiale, mais cela dépend du nombre de processeurs graphiques que vous avez mis à disposition. 

- Si un processeur graphique est mis à disposition, vous pouvez en ajouter un autre, ou
- Si deux processeurs graphiques sont mis à disposition, vous pouvez revenir à un seul processeur graphique.
