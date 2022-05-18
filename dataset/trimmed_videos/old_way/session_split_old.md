# Splits based on session

## Trimmed videos


<a id="org3418b05"></a>

### Creation:

This dataset is created by trimming a 3 second instance from middle of
activity instance (ground truth). Trimmed videos are then resized to 224
pixels on the longer edge(the aspect ratio).


<a id="orga2747b1"></a>

### Properties:

-   Shape: The longer edge is resized to 224
-   Frame rate: 30 FPS


<a id="orgfe6d13e"></a>

## Session based splits


<a id="org17c8144"></a>

### typing, notyping


<a id="orgc169a10"></a>

#### Training

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
<caption class="t-above"><span class="table-number">Table 1:</span> Table demonstrating diversity in training dataset</caption>

<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-right">No. samples per activity</th>
<th scope="col" class="org-right">No. groups</th>
<th scope="col" class="org-right">No. Sessions</th>
<th scope="col" class="org-right">No. Persons</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-right">25</td>
<td class="org-right">7</td>
<td class="org-right">20</td>
<td class="org-right">18</td>
</tr>


<tr>
<td class="org-right">50</td>
<td class="org-right">10</td>
<td class="org-right">30</td>
<td class="org-right">32</td>
</tr>


<tr>
<td class="org-right">75</td>
<td class="org-right">10</td>
<td class="org-right">33</td>
<td class="org-right">35</td>
</tr>


<tr>
<td class="org-right">100</td>
<td class="org-right">10</td>
<td class="org-right">33</td>
<td class="org-right">35</td>
</tr>


<tr>
<td class="org-right">125</td>
<td class="org-right">10</td>
<td class="org-right">33</td>
<td class="org-right">35</td>
</tr>


<tr>
<td class="org-right">142</td>
<td class="org-right">10</td>
<td class="org-right">33</td>
<td class="org-right">35</td>
</tr>


<tr>
<td class="org-right">all *(142 ntyp, 262 typ)*</td>
<td class="org-right">10</td>
<td class="org-right">33</td>
<td class="org-right">35</td>
</tr>
</tbody>
</table>

Sessions:

    'G-C1L1P-Apr06-A' 'G-C1L1P-Apr06-B' 'G-C1L1P-Apr06-D' 'G-C1L1P-Apr13-A'
    'G-C1L1P-Apr13-D' 'G-C1L1P-Apr20-A' 'G-C1L1P-Apr20-C' 'G-C1L1P-Apr20-D'
    'G-C1L1P-Apr27-B' 'G-C1L1P-Feb16-A' 'G-C1L1P-Feb16-C' 'G-C1L1P-Feb25-A'
    'G-C1L1P-Feb25-C' 'G-C1L1P-Feb25-E' 'G-C1L1P-Mar02-A' 'G-C1L1P-Mar02-C'
    'G-C1L1P-Mar09-A' 'G-C1L1P-Mar09-B' 'G-C1L1P-Mar09-C' 'G-C1L1P-Mar09-D'
    'G-C1L1P-Mar30-B' 'G-C1L1P-May04-B' 'G-C1L1P-May06-B' 'G-C1L1P-May11-B'
    'G-C1L1W-Apr25-A' 'G-C1L1W-Feb21-A' 'G-C1L1W-Feb21-C' 'G-C1L1W-Feb28-A'
    'G-C1L1W-Feb28-D' 'G-C1L1W-Mar07-A' 'G-C1L1W-Mar28-A' 'G-C1L1W-May06-B'
    'G-C2L1W-Apr10-A'


<a id="orgd9a2395"></a>

#### Validation

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
<caption class="t-above"><span class="table-number">Table 2:</span> Table demonstrating diversity in validation dataset</caption>

<colgroup>
<col  class="org-left" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">No. samples per activity</th>
<th scope="col" class="org-right">No. groups</th>
<th scope="col" class="org-right">No. Sessions</th>
<th scope="col" class="org-right">No. Persons</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-left">50 split 1 *(25, 25)*</td>
<td class="org-right">5</td>
<td class="org-right">5</td>
<td class="org-right">13</td>
</tr>


<tr>
<td class="org-left">50 split 2 *(25, 25)*</td>
<td class="org-right">5</td>
<td class="org-right">5</td>
<td class="org-right">11</td>
</tr>


<tr>
<td class="org-left">50</td>
<td class="org-right">5</td>
<td class="org-right">5</td>
<td class="org-right">13</td>
</tr>


<tr>
<td class="org-left">all split1 *(104 ntyp, 88 typ)*</td>
<td class="org-right">5</td>
<td class="org-right">5</td>
<td class="org-right">13</td>
</tr>


<tr>
<td class="org-left">all split2 *(104 ntyp, 88 typ)*</td>
<td class="org-right">3</td>
<td class="org-right">3</td>
<td class="org-right">8</td>
</tr>


<tr>
<td class="org-left">all *(208 ntyp, 176 typ)*</td>
<td class="org-right">5</td>
<td class="org-right">5</td>
<td class="org-right">13</td>
</tr>
</tbody>
</table>

Sessions:

    'G-C1L1P-Mar02-B' 'G-C1L1P-May04-C' 'G-C2L1P-Apr12-C' 'G-C2L1W-Feb27-B'
    'G-C3L1W-Mar19-D'


<a id="org1713721"></a>

#### Testing

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
<caption class="t-above"><span class="table-number">Table 3:</span> Table demonstrating diversity in testing dataset</caption>

<colgroup>
<col  class="org-left" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">No. samples per activity</th>
<th scope="col" class="org-right">No. groups</th>
<th scope="col" class="org-right">No. Sessions</th>
<th scope="col" class="org-right">No. Persons</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-left">all *(298 ntyp, 239 typ)*</td>
<td class="org-right">6</td>
<td class="org-right">7</td>
<td class="org-right">24</td>
</tr>
</tbody>
</table>

Sessions:

    'G-C1L1P-Apr13-C' 'G-C1L1P-Mar02-E' 'G-C1L1P-Mar30-C' 'G-C2L1P-Feb23-B'
    'G-C2L1P-Mar08-D' 'G-C3L1P-Apr11-C' 'G-C3L1P-Feb21-D'


<a id="orga90f77a"></a>

### writing, nowriting


<a id="orgcb14f14"></a>

#### Training

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
<caption class="t-above"><span class="table-number">Table 4:</span> Table demonstrating diversity in training dataset</caption>

<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">No. samples per activity</td>
<td class="org-right">No. groups</td>
<td class="org-right">No. Sessions</td>
<td class="org-right">No. Persons</td>
</tr>


<tr>
<td class="org-right">25</td>
<td class="org-right">7</td>
<td class="org-right">18</td>
<td class="org-right">24</td>
</tr>


<tr>
<td class="org-right">50</td>
<td class="org-right">7</td>
<td class="org-right">22</td>
<td class="org-right">27</td>
</tr>


<tr>
<td class="org-right">75</td>
<td class="org-right">7</td>
<td class="org-right">22</td>
<td class="org-right">32</td>
</tr>


<tr>
<td class="org-right">100</td>
<td class="org-right">7</td>
<td class="org-right">22</td>
<td class="org-right">32</td>
</tr>


<tr>
<td class="org-right">125</td>
<td class="org-right">7</td>
<td class="org-right">22</td>
<td class="org-right">32</td>
</tr>


<tr>
<td class="org-right">150</td>
<td class="org-right">7</td>
<td class="org-right">22</td>
<td class="org-right">32</td>
</tr>


<tr>
<td class="org-right">all *(193 nw, 792 w)*</td>
<td class="org-right">7</td>
<td class="org-right">22</td>
<td class="org-right">32</td>
</tr>
</tbody>
</table>

Sessions:

    'G-C1L1P-Apr06-C' 'G-C1L1P-Apr06-D' 'G-C1L1P-Apr13-D' 'G-C1L1P-Apr20-C'
    'G-C1L1P-Apr20-D' 'G-C1L1P-Feb16-C' 'G-C1L1P-Feb25-C' 'G-C1L1P-Mar02-D'
    'G-C1L1P-Mar09-C' 'G-C1L1P-Mar09-D' 'G-C1L1P-Mar30-C' 'G-C1L1P-Mar30-D'
    'G-C1L1P-May11-C' 'G-C1L1W-Apr04-A' 'G-C1L1W-Feb14-A' 'G-C1L1W-Feb21-A'
    'G-C1L1W-Feb28-A' 'G-C2L1P-Feb23-B' 'G-C2L1W-Apr10-A' 'G-C2L1W-Feb20-A'
    'G-C2L1W-Feb27-B' 'G-C3L1P-Feb14-D'


<a id="orgb358d43"></a>

#### Validation

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
<caption class="t-above"><span class="table-number">Table 5:</span> Table demonstrating diversity in validation dataset</caption>

<colgroup>
<col  class="org-left" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-left">No. samples per activity</td>
<td class="org-right">No. groups</td>
<td class="org-right">No. Sessions</td>
<td class="org-right">No. Persons</td>
</tr>


<tr>
<td class="org-left">50 split1 *(25, 25)*</td>
<td class="org-right">4</td>
<td class="org-right">4</td>
<td class="org-right">15</td>
</tr>


<tr>
<td class="org-left">50 split2 *(25, 25)*</td>
<td class="org-right">4</td>
<td class="org-right">4</td>
<td class="org-right">14</td>
</tr>


<tr>
<td class="org-left">50</td>
<td class="org-right">4</td>
<td class="org-right">4</td>
<td class="org-right">15</td>
</tr>


<tr>
<td class="org-left">all split1 *(58 nw, 91 w)*</td>
<td class="org-right">4</td>
<td class="org-right">4</td>
<td class="org-right">15</td>
</tr>


<tr>
<td class="org-left">all split2 *(58 nw, 90 w)*</td>
<td class="org-right">4</td>
<td class="org-right">4</td>
<td class="org-right">11</td>
</tr>


<tr>
<td class="org-left">all *(116 nw, 181 w)*</td>
<td class="org-right">4</td>
<td class="org-right">4</td>
<td class="org-right">15</td>
</tr>
</tbody>
</table>

Sessions:

    'G-C1L1P-Mar02-B' 'G-C1L1P-May04-C' 'G-C2L1P-Apr12-C' 'G-C3L1W-Mar19-D'


<a id="org017ecf4"></a>

#### Testing

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
<caption class="t-above"><span class="table-number">Table 6:</span> Table demonstrating diversity in testing dataset</caption>

<colgroup>
<col  class="org-left" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-left">No. samples per activity</td>
<td class="org-right">No. groups</td>
<td class="org-right">No. Sessions</td>
<td class="org-right">No. Persons</td>
</tr>


<tr>
<td class="org-left">all *(489 nw, 271 w)*</td>
<td class="org-right">6</td>
<td class="org-right">6</td>
<td class="org-right">22</td>
</tr>
</tbody>
</table>

Sessions:

    'G-C1L1P-Apr13-C' 'G-C1L1P-Mar02-E' 'G-C2L1P-Apr12-E' 'G-C2L1P-Mar08-D'
    'G-C3L1P-Apr11-C' 'G-C3L1P-Feb21-D'

