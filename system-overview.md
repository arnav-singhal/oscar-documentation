# System Hardware

## Oscar Specifications

|                        |       |
| ---------------------- | ----- |
| **Compute Nodes**      | 461   |
| **Total CPU Cores**    | 17424 |
| **GPU Nodes**          | 69    |
| **Total GPUs**         | 474   |
| **Large Memory Nodes** | 4     |

## Compute Nodes

Oscar has compute nodes in the partitions listed below.

* **batch** - The batch partition is for programs/jobs which need neither GPUs nor large memory.
* **bigmem** - The bigmem partition is for programs/jobs which require large memory.&#x20;
* **debug** - The debug partition is for users to debug programs/jobs.
* **gpu** - The gpu partition is for programs/jobs which require GPUs.
* **gpu-debug** - The gpu-debug partition is for users to debug gpu programs/jobs.&#x20;
* **gpu-he** -The gpu-he partition is for programs/jobs which need to access high-end GPUs.&#x20;
* **vnc** - The vnc partition is for users to run programs/jobs in an graphical desktop environment.&#x20;

Below are node details including cores and memory for all partitions.

<table data-header-hidden><thead><tr><th></th><th></th><th></th><th></th><th width="101"></th><th></th></tr></thead><tbody><tr><td><strong>Partition</strong></td><td><strong>Total</strong><br><strong>Nodes</strong></td><td><strong>Total</strong><br><strong>Cores</strong></td><td><strong>Cores</strong><br><strong>Per Node</strong></td><td><strong>Total</strong><br><strong>GPUs</strong></td><td><strong>Memory Per</strong><br><strong>Node (GB)</strong></td></tr><tr><td>batch</td><td>384</td><td>14272</td><td>24-48</td><td>n/a</td><td>95-385</td></tr><tr><td>bigmem</td><td>4</td><td>128</td><td>32</td><td>n/a</td><td>772-2146</td></tr><tr><td>gpu</td><td>46</td><td>2216</td><td>8-64</td><td>358</td><td>95-1030</td></tr><tr><td>gpu-he</td><td>12</td><td>552</td><td>24-64</td><td>84</td><td>192-1030</td></tr><tr><td>debug</td><td>4</td><td>96</td><td>24</td><td>n/a</td><td>95</td></tr><tr><td>gpu-debug</td><td>3</td><td>24</td><td>8</td><td>12</td><td>192</td></tr><tr><td>vnc</td><td>25</td><td>584</td><td>8-32</td><td>22</td><td>95-773</td></tr><tr><td>viz</td><td>2</td><td>16</td><td>8</td><td>8</td><td>192</td></tr></tbody></table>

## Hardware details

Hardware details for all partitions. The Features column shows the features available for the --constraint option for SLURM. This includes the available CPU types as well GPUs.

<table><thead><tr><th width="112">Partition</th><th width="77">CPUs/ Node</th><th width="71">Nodes</th><th width="77">Total CPUs</th><th width="63">GPUs/ Node</th><th width="75">Total GPUs</th><th width="72">Memory (GB)</th><th>Features</th></tr></thead><tbody><tr><td>batch</td><td>48</td><td>164</td><td>7872</td><td>n/a</td><td>n/a</td><td>385</td><td>48core, intel, cascade, edr</td></tr><tr><td>batch</td><td>32</td><td>40</td><td>1280</td><td>n/a</td><td>n/a</td><td>385</td><td>32core, intel, scalable, cascade, edr</td></tr><tr><td>batch</td><td>24</td><td>34</td><td>816</td><td>n/a</td><td>n/a</td><td>192</td><td>24core, intel, e5-2670, e5-2600, scalable, skylake, fdr</td></tr><tr><td>batch</td><td>24</td><td>42</td><td>1008</td><td>n/a</td><td>n/a</td><td>95</td><td>24core, intel, e5-2670, e5-2600, scalable, skylake, fdr</td></tr><tr><td>batch</td><td>24</td><td>4</td><td>96</td><td>n/a</td><td>n/a</td><td>385</td><td>24core, intel, e5-2670, e5-2600, scalable, skylake, fdr</td></tr><tr><td>batch</td><td>32</td><td>100</td><td>3200</td><td>n/a</td><td>n/a</td><td>192</td><td>32core, intel, scalable, cascade, edr</td></tr><tr><td>bigmem</td><td>32</td><td>2</td><td>64</td><td>n/a</td><td>n/a</td><td>772</td><td>32core, intel, scalable, cascade, edr</td></tr><tr><td>bigmem</td><td>32</td><td>2</td><td>64</td><td>n/a</td><td>n/a</td><td>2146</td><td>32core, intel, scalable, cascade, edr</td></tr><tr><td>gpu</td><td>64</td><td>2</td><td>128</td><td>8</td><td>16</td><td>1030</td><td>amd, gpu, geforce3090, ampere</td></tr><tr><td>gpu</td><td>32</td><td>2</td><td>64</td><td>5</td><td>10</td><td>385</td><td>intel, gpu, titanrtx, turing, skylake, 6142</td></tr><tr><td>gpu</td><td>24</td><td>1</td><td>24</td><td>5</td><td>5</td><td>192</td><td>intel, gpu, titanrtx, turing, skylake, 6142</td></tr><tr><td>gpu</td><td>48</td><td>1</td><td>48</td><td>10</td><td>10</td><td>385</td><td>intel, gpu, quadrortx, turing, cascade</td></tr><tr><td>gpu</td><td>32</td><td>10</td><td>320</td><td>10</td><td>100</td><td>385</td><td>intel, gpu, quadrortx, turing, cascade</td></tr><tr><td>gpu</td><td>64</td><td>10</td><td>640</td><td>8</td><td>80</td><td>1030</td><td>amd, gpu, geforce3090, ampere</td></tr><tr><td>gpu</td><td>64</td><td>1</td><td>64</td><td>7</td><td>7</td><td>1030</td><td>amd, gpu, geforce3090, ampere</td></tr><tr><td>gpu</td><td>48</td><td>4</td><td>192</td><td>8</td><td>32</td><td>1030</td><td>amd, gpu, geforce3090, ampere</td></tr><tr><td>gpu</td><td>64</td><td>10</td><td>640</td><td>8</td><td>80</td><td>1030</td><td>amd, gpu, a5000, ampere</td></tr><tr><td>gpu</td><td>8</td><td>4</td><td>32</td><td>4</td><td>16</td><td>95</td><td>intel, gpu, titanv, volta, skylake, 5122</td></tr><tr><td>gpu</td><td>64</td><td>1</td><td>64</td><td>2</td><td>2</td><td>1030</td><td>amd, gpu, a5000, ampere</td></tr><tr><td>gpu-he</td><td>48</td><td>1</td><td>48</td><td>8</td><td>8</td><td>1030</td><td>amd, gpu, a40, ampere</td></tr><tr><td>gpu-he</td><td>48</td><td>2</td><td>96</td><td>8</td><td>16</td><td>1030</td><td>amd, gpu, a40, ampere</td></tr><tr><td>gpu-he</td><td>24</td><td>3</td><td>72</td><td>4</td><td>12</td><td>192</td><td>intel, gpu, 4gpu, v100, volta, skylake, 6126</td></tr><tr><td>gpu-he</td><td>40</td><td>2</td><td>80</td><td>8</td><td>16</td><td>515</td><td>intel, gpu, v100, volta, haswell</td></tr><tr><td>gpu-he</td><td>64</td><td>4</td><td>256</td><td>8</td><td>32</td><td>1030</td><td>amd, gpu, a6000, ampere</td></tr><tr><td>debug</td><td>24</td><td>4</td><td>96</td><td>n/a</td><td>n/a</td><td>95</td><td>24core, intel, e5-2670, e5-2600, scalable, skylake, fdr</td></tr><tr><td>gpu-debug</td><td>8</td><td>3</td><td>24</td><td>4</td><td>12</td><td>192</td><td>gpu, p100, pascal</td></tr><tr><td>vnc</td><td>32</td><td>2</td><td>64</td><td>7</td><td>14</td><td>773</td><td>gpu, 1080ti, pascal</td></tr><tr><td>vnc</td><td>8</td><td>2</td><td>16</td><td>4</td><td>8</td><td>192</td><td>gpu, p100, pascal</td></tr><tr><td>vnc</td><td>24</td><td>21</td><td>504</td><td>n/a</td><td>n/a</td><td>95</td><td>24core, intel, e5-2670, e5-2600, scalable, skylake, fdr</td></tr><tr><td>viz</td><td>8</td><td>2</td><td>16</td><td>4</td><td>8</td><td>192</td><td>gpu, p100, pascal</td></tr></tbody></table>

## GPU Features and GPU Memory

<table><thead><tr><th width="333.3333333333333">GPU Features</th><th>GPU Memory</th></tr></thead><tbody><tr><td>a6000</td><td>48 GB</td></tr><tr><td>a40</td><td>45 GB</td></tr><tr><td>v100</td><td>32 GB</td></tr><tr><td>a5000</td><td>24 GB</td></tr><tr><td>quadrortx</td><td>24 GB</td></tr><tr><td>titanrtx</td><td>24 GB</td></tr><tr><td>geforce3090</td><td>24 GB</td></tr><tr><td>p100</td><td>12 GB</td></tr><tr><td>titanv</td><td>12 GB</td></tr><tr><td>1000ti</td><td>11 GB</td></tr><tr><td></td><td></td></tr></tbody></table>

