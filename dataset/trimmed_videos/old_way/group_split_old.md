# Splits based on groups

## Trimmed videos


<a id="org1643656"></a>

### Creation:

This dataset is created by trimming a 3 second instance from middle of
activity instance (ground truth). Trimmed videos are then resized to 224
pixels on the longer edge(the aspect ratio).


<a id="org013803c"></a>

### Properties:

-   Shape: The longer edge is resized to 224
-   Frame rate: 30 FPS


<a id="orgb153d70"></a>

## Group based splits


<a id="org0c5bfee"></a>

### typing/notyping

Table [1](#org65d5beb)summarize all the groups that have samples 
available for *typing/notyping*. From these groups we perform leave one out 
on the ones that have reasonable number of samples marked with \*.

---

<table id="org65d5beb" border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
<caption class="t-above"><span class="table-number">Table 1:</span> *typing/notyping* dataset samples per group.</caption>

<colgroup>
<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">Group</th>
<th scope="col" class="org-left"># Samples (ty, nty)</th>
<th scope="col" class="org-left">Used?</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-left">C1L1P-A \*</td>
<td class="org-left">33, 39</td>
<td class="org-left">Yes</td>
</tr>


<tr>
<td class="org-left">C1L1P-B \*</td>
<td class="org-left">55, 40</td>
<td class="org-left">Yes</td>
</tr>


<tr>
<td class="org-left">C1L1P-C \*</td>
<td class="org-left">109, 83</td>
<td class="org-left">Yes</td>
</tr>


<tr>
<td class="org-left">C1L1P-D</td>
<td class="org-left">57, 3</td>
<td class="org-left">No</td>
</tr>


<tr>
<td class="org-left">C1L1P-E</td>
<td class="org-left">6, 4</td>
<td class="org-left">No</td>
</tr>


<tr>
<td class="org-left">C1L1W-A \*</td>
<td class="org-left">30, 18</td>
<td class="org-left">Yes</td>
</tr>


<tr>
<td class="org-left">C1L1W-B</td>
<td class="org-left">9, 2</td>
<td class="org-left">No</td>
</tr>


<tr>
<td class="org-left">C1L1W-C</td>
<td class="org-left">3, 2</td>
<td class="org-left">No</td>
</tr>


<tr>
<td class="org-left">C1L1W-D</td>
<td class="org-left">4, 2</td>
<td class="org-left">No</td>
</tr>


<tr>
<td class="org-left">C2L1W-A</td>
<td class="org-left">2, 5</td>
<td class="org-left">No</td>
</tr>


<tr>
<td class="org-left">C2L1P-C</td>
<td class="org-left">6, 0</td>
<td class="org-left">No</td>
</tr>


<tr>
<td class="org-left">C2L1W-B \*</td>
<td class="org-left">75, 80</td>
<td class="org-left">Yes</td>
</tr>


<tr>
<td class="org-left">C3L1W-D \*</td>
<td class="org-left">49, 72</td>
<td class="org-left">Yes</td>
</tr>
</tbody>
</table>

Table [2](#orgf4d74e5) provides training and validation
samples for each leave one out loop using groups.

<table id="orgf4d74e5" border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
<caption class="t-above"><span class="table-number">Table 2:</span> Training and validation samples for each left out group.</caption>

<colgroup>
<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">Group</th>
<th scope="col" class="org-left"># Training samples</th>
<th scope="col" class="org-left"># Validation samples</th>
</tr>


<tr>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">(ty, nty)</th>
<th scope="col" class="org-left">(ty, nty)</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-left">C1L1P-A</td>
<td class="org-left">318, 293</td>
<td class="org-left">33, 39</td>
</tr>


<tr>
<td class="org-left">C1L1P-B</td>
<td class="org-left">296, 292</td>
<td class="org-left">55, 40</td>
</tr>


<tr>
<td class="org-left">C1L1P-C</td>
<td class="org-left">242, 249</td>
<td class="org-left">109, 83</td>
</tr>


<tr>
<td class="org-left">C1L1W-A</td>
<td class="org-left">321, 314</td>
<td class="org-left">30, 18</td>
</tr>


<tr>
<td class="org-left">C2L1W-B</td>
<td class="org-left">276, 252</td>
<td class="org-left">75, 80</td>
</tr>


<tr>
<td class="org-left">C3L1W-D</td>
<td class="org-left">302, 260</td>
<td class="org-left">49, 72</td>
</tr>
</tbody>
</table>


<a id="org9b49f7a"></a>

### writing/nowriting

Table [3](#org1373a9d)summarize all the groups that have samples 
available for *writing/nowriting*. From these groups we perform leave one out 
on the ones that have reasonable number of samples marked with \*.

<table id="org1373a9d" border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
<caption class="t-above"><span class="table-number">Table 3:</span> *writing/nowriting* dataset samples per group.</caption>

<colgroup>
<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">groups</th>
<th scope="col" class="org-left"># Samples</th>
<th scope="col" class="org-left">Used?</th>
</tr>


<tr>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">w, nw</th>
<th scope="col" class="org-left">&#xa0;</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-left">C1L1P-B \*</td>
<td class="org-left">57,75</td>
<td class="org-left">Yes</td>
</tr>


<tr>
<td class="org-left">C1L1P-C \*</td>
<td class="org-left">337, 138</td>
<td class="org-left">Yes</td>
</tr>


<tr>
<td class="org-left">C1L1P-D</td>
<td class="org-left">172, 1</td>
<td class="org-left">No</td>
</tr>


<tr>
<td class="org-left">C1L1W-A</td>
<td class="org-left">155, 0</td>
<td class="org-left">No</td>
</tr>


<tr>
<td class="org-left">C2L1P-B \*</td>
<td class="org-left">17, 56</td>
<td class="org-left">Yes</td>
</tr>


<tr>
<td class="org-left">C2L1P-C \*</td>
<td class="org-left">88, 35</td>
<td class="org-left">Yes</td>
</tr>


<tr>
<td class="org-left">C2L1W-A</td>
<td class="org-left">116, 0</td>
<td class="org-left">No</td>
</tr>


<tr>
<td class="org-left">C2L1W-B</td>
<td class="org-left">11, 0</td>
<td class="org-left">No</td>
</tr>


<tr>
<td class="org-left">C3L1P-D</td>
<td class="org-left">2, 0</td>
<td class="org-left">No</td>
</tr>


<tr>
<td class="org-left">C3L1W-D</td>
<td class="org-left">18, 4</td>
<td class="org-left">No</td>
</tr>
</tbody>
</table>

Table [4](#org07c8557) provides training and validation
samples for each group.

<table id="org07c8557" border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
<caption class="t-above"><span class="table-number">Table 4:</span> Training and validation samples for each left out group.</caption>

<colgroup>
<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">groups</th>
<th scope="col" class="org-left"># Training samples</th>
<th scope="col" class="org-left"># Validation samples</th>
</tr>


<tr>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">w, nw</th>
<th scope="col" class="org-left">w, nw</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-left">C1L1P-B \*</td>
<td class="org-left">442, 229</td>
<td class="org-left">57,75</td>
</tr>


<tr>
<td class="org-left">C1L1P-C \*</td>
<td class="org-left">162, 166</td>
<td class="org-left">337, 138</td>
</tr>


<tr>
<td class="org-left">C2L1P-B \*</td>
<td class="org-left">482, 248</td>
<td class="org-left">17, 56</td>
</tr>


<tr>
<td class="org-left">C2L1P-C \*</td>
<td class="org-left">411, 269</td>
<td class="org-left">88, 35</td>
</tr>
</tbody>
</table>

