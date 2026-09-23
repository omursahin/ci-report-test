<a name="wfc-top"></a>

## &#x274C; Found 529 potential faults

<sub>WFC report schema 0.0.1 &middot; created 2025-04-09T19:31:54.258Z</sub>

> [!CAUTION]
> **529 potential faults** &middot; 1 fault type &middot; 62/67 endpoints affected &middot; 127 test cases &middot; &#x23F1; 1883h 20m 0s

[Faults](#user-content-wfc-faults) &middot; [Endpoints](#user-content-wfc-endpoints) &middot; [Tests](#user-content-wfc-tests) &middot; [Interactive report](https://github.com/omursahin/ci-report-test/actions/runs/1/artifacts/2)

> [!TIP]
> **Interactive report:** [download the artifact](https://github.com/omursahin/ci-report-test/actions/runs/1/artifacts/2), unzip it and open `low-code-index.html` in a browser.
>
> **Workflow run:** [https://github.com/omursahin/ci-report-test/actions/runs/1](https://github.com/omursahin/ci-report-test/actions/runs/1)

### Overview

| Metric | Value |
| --- | --- |
| Endpoints | 67 |
| Test files | 2 |
| Test cases | 127 |
| HTTP calls in generated tests | 25 |
| HTTP calls evaluated during fuzzing | 132 |
| Potential faults | 529 |
| Distinct fault types | 1 |
| Execution time | 1883h 20m 0s |

### Endpoint status coverage

Endpoints for which at least one generated test received a response in the given status class.

| Status | Endpoints | Ratio |
| --- | --- | --- |
| 2XX | 27/67 | <code>&#x2588;&#x2588;&#x2588;&#x2588;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;</code> 40% |
| 3XX | 0/67 | <code>&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;</code> 0% |
| 4XX | 55/67 | <code>&#x2588;&#x2588;&#x2588;&#x2588;&#x2588;&#x2588;&#x2588;&#x2588;&#x2591;&#x2591;</code> 82% |
| 5XX | 0/67 | <code>&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;</code> 0% |

### Code coverage

| Criterion | Covered | Total | Ratio |
| --- | --- | --- | --- |
| Line Coverage | 428 | 1229 | <code>&#x2588;&#x2588;&#x2588;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;</code> 35% |
| Branch Coverage | 6 | 130 | <code>&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;&#x2591;</code> 5% |

<a name="wfc-faults"></a>

### Faults by category

| Code | Name | Affected endpoints | Faults |
| --- | --- | --- | --- |
| F200 | Schema Violation: Received A Response From API With A Structure/Data That Is Not Matching Its Schema | 62/67 | 529 |

### Warnings (1)

> [!WARNING]
> - **FUZZER**: No authentication info was provided. Unless you are testing an example API, you should setup some authentication info for different users. If this is the first time you are using EvoMaster, and you just want to get a feeling of how it works, then ignore this warning. However, to get better results, you will need setup authentication info, eventually. More info is currently available at https://github.com/WebFuzzing/EvoMaster/blob/master/docs/auth.md

### Fault details (529)

<details>
<summary><b>F200</b> Schema Violation: Received A Response From API With A Structure/Data That Is Not Matching Its Schema &middot; 529 faults on 62 endpoints</summary>

| Operation | Faults | Example | Test cases |
| --- | --- | --- | --- |
| <code>GET:/app/api/assignments</code> | 192 | \[Path '/collection/0/commitEmpDesc'\] Instance type (null) does not match any allowed primitive type (allowed: \["string"\]) | [<code>faults.java#test\_16</code>](#user-content-test-faults-java-test-16) |
| <code>GET:/app/api/assignments/</code> | 192 | \[Path '/collection/0/commitEmpDesc'\] Instance type (null) does not match any allowed primitive type (allowed: \["string"\]) | [<code>faults.java#test\_17</code>](#user-content-test-faults-java-test-17) |
| <code>GET:/app/api/employees</code> | 33 | \[Path '/collection/0/manager/hiredate'\] Instance type (null) does not match any allowed primitive type (allowed: \["string"\]) | [<code>faults.java#test\_12</code>](#user-content-test-faults-java-test-12) |
| <code>GET:/app/api/employees/</code> | 33 | \[Path '/collection/0/manager/hiredate'\] Instance type (null) does not match any allowed primitive type (allowed: \["string"\]) | [<code>faults.java#test\_13</code>](#user-content-test-faults-java-test-13) |
| <code>GET:/app/api/credentials</code> | 6 | \[Path '/collection/14/password'\] Instance type (null) does not match any allowed primitive type (allowed: \["string"\]) | [<code>faults.java#test\_11</code>](#user-content-test-faults-java-test-11) |
| <code>GET:/app/api/employees/data/manager-project-data/{employeeId}</code> | 4 | \[Path '/collection/0/title'\] Instance type (null) does not match any allowed primitive type (allowed: \["string"\]) | [<code>faults.java#test\_5</code>](#user-content-test-faults-java-test-5), [<code>faults.java#test\_32</code>](#user-content-test-faults-java-test-32) |
| <code>POST:/app/api/credentials</code> | 4 | \[Path '/password'\] Instance type (null) does not match any allowed primitive type (allowed: \["string"\]) | [<code>faults.java#test\_7</code>](#user-content-test-faults-java-test-7), [<code>faults.java#test\_6</code>](#user-content-test-faults-java-test-6), [<code>faults.java#test\_11</code>](#user-content-test-faults-java-test-11) (+1 more) |
| <code>POST:/app/api/credentials/save</code> | 4 | \[Path '/password'\] Instance type (null) does not match any allowed primitive type (allowed: \["string"\]) | [<code>faults.java#test\_4</code>](#user-content-test-faults-java-test-4), [<code>faults.java#test\_87</code>](#user-content-test-faults-java-test-87) |
| <code>POST:/app/api/departments</code> | 3 | \[Path '/location/adr'\] Instance type (null) does not match any allowed primitive type (allowed: \["string"\]) | [<code>faults.java#test\_9</code>](#user-content-test-faults-java-test-9), [<code>faults.java#test\_3</code>](#user-content-test-faults-java-test-3), [<code>faults.java#test\_79</code>](#user-content-test-faults-java-test-79) (+1 more) |
| <code>POST:/app/api/projects</code> | 3 | \[Path '/endDate'\] Instance type (null) does not match any allowed primitive type (allowed: \["string"\]) | [<code>faults.java#test\_15</code>](#user-content-test-faults-java-test-15), [<code>faults.java#test\_10</code>](#user-content-test-faults-java-test-10), [<code>faults.java#test\_19</code>](#user-content-test-faults-java-test-19) (+2 more) |
| <code>GET:/app/api/credentials/</code> | 2 | \[Path '/collection/14/role'\] Instance type (null) does not match any allowed primitive type (allowed: \["string"\]) | [<code>faults.java#test\_0</code>](#user-content-test-faults-java-test-0) |
| <code>GET:/app/api/projects</code> | 2 | \[Path '/collection/9/endDate'\] Instance type (null) does not match any allowed primitive type (allowed: \["string"\]) | [<code>faults.java#test\_1</code>](#user-content-test-faults-java-test-1), [<code>faults.java#test\_2</code>](#user-content-test-faults-java-test-2) |
| <code>PUT:/app/api/credentials/update</code> | 2 | \[Path '/username'\] Instance type (null) does not match any allowed primitive type (allowed: \["string"\]) | [<code>faults.java#test\_8</code>](#user-content-test-faults-java-test-8), [<code>faults.java#test\_88</code>](#user-content-test-faults-java-test-88) |
| <code>DELETE:/app/api/assignments/{employeeId}/{projectId}/{commitDate}</code> | 1 | Response status 400 not defined for path '/api/assignments/{employeeId}/{projectId}/{commitDate}'. | [<code>faults.java#test\_65</code>](#user-content-test-faults-java-test-65) |
| <code>DELETE:/app/api/assignments/delete/{employeeId}/{projectId}/{commitDate}</code> | 1 | Response status 400 not defined for path '/api/assignments/delete/{employeeId}/{projectId}/{commitDate}'. | [<code>faults.java#test\_21</code>](#user-content-test-faults-java-test-21) |
| <code>DELETE:/app/api/credentials/{id}</code> | 1 | Response status 400 not defined for path '/api/credentials/{id}'. | [<code>faults.java#test\_71</code>](#user-content-test-faults-java-test-71), [<code>faults.java#test\_91</code>](#user-content-test-faults-java-test-91) |
| <code>DELETE:/app/api/credentials/delete/{id}</code> | 1 | Response status 400 not defined for path '/api/credentials/delete/{id}'. | [<code>faults.java#test\_33</code>](#user-content-test-faults-java-test-33) |
| <code>DELETE:/app/api/credentials/username/{username}</code> | 1 | Response status 400 not defined for path '/api/credentials/username/{username}'. | [<code>faults.java#test\_38</code>](#user-content-test-faults-java-test-38) |
| <code>DELETE:/app/api/departments/{id}</code> | 1 | Response status 400 not defined for path '/api/departments/{id}'. | [<code>faults.java#test\_67</code>](#user-content-test-faults-java-test-67) |
| <code>DELETE:/app/api/departments/delete/{id}</code> | 1 | Response status 400 not defined for path '/api/departments/delete/{id}'. | [<code>faults.java#test\_23</code>](#user-content-test-faults-java-test-23) |
| <code>DELETE:/app/api/employees/{id}</code> | 1 | Response status 400 not defined for path '/api/employees/{id}'. | [<code>faults.java#test\_24</code>](#user-content-test-faults-java-test-24) |
| <code>DELETE:/app/api/employees/delete/{id}</code> | 1 | Response status 400 not defined for path '/api/employees/delete/{id}'. | [<code>faults.java#test\_72</code>](#user-content-test-faults-java-test-72) |
| <code>DELETE:/app/api/employees/username/{username}</code> | 1 | Response status 400 not defined for path '/api/employees/username/{username}'. | [<code>faults.java#test\_59</code>](#user-content-test-faults-java-test-59), [<code>faults.java#test\_62</code>](#user-content-test-faults-java-test-62) |
| <code>DELETE:/app/api/locations/{id}</code> | 1 | Response status 400 not defined for path '/api/locations/{id}'. | [<code>faults.java#test\_68</code>](#user-content-test-faults-java-test-68) |
| <code>DELETE:/app/api/locations/delete/{id}</code> | 1 | Response status 400 not defined for path '/api/locations/delete/{id}'. | [<code>faults.java#test\_25</code>](#user-content-test-faults-java-test-25) |
| <code>DELETE:/app/api/projects/{id}</code> | 1 | Response status 400 not defined for path '/api/projects/{id}'. | [<code>faults.java#test\_37</code>](#user-content-test-faults-java-test-37), [<code>faults.java#test\_56</code>](#user-content-test-faults-java-test-56) |
| <code>DELETE:/app/api/projects/delete/{id}</code> | 1 | Response status 400 not defined for path '/api/projects/delete/{id}'. | [<code>faults.java#test\_26</code>](#user-content-test-faults-java-test-26) |
| <code>GET:/app/api/assignments/{employeeId}/{projectId}</code> | 1 | Response status 400 not defined for path '/api/assignments/{employeeId}/{projectId}'. | [<code>faults.java#test\_18</code>](#user-content-test-faults-java-test-18) |
| <code>GET:/app/api/assignments/{employeeId}/{projectId}/{commitDate}</code> | 1 | Response status 400 not defined for path '/api/assignments/{employeeId}/{projectId}/{commitDate}'. | [<code>faults.java#test\_31</code>](#user-content-test-faults-java-test-31) |
| <code>GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}</code> | 1 | Response status 400 not defined for path '/api/assignments/data/project-commit/{employeeId}/{projectId}'. | [<code>faults.java#test\_30</code>](#user-content-test-faults-java-test-30), [<code>faults.java#test\_64</code>](#user-content-test-faults-java-test-64), [<code>faults.java#test\_70</code>](#user-content-test-faults-java-test-70) |
| <code>GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}/{commitDate}</code> | 1 | Response status 400 not defined for path '/api/assignments/data/project-commit/{employeeId}/{projectId}/{commitDate}'. | [<code>faults.java#test\_63</code>](#user-content-test-faults-java-test-63), [<code>faults.java#test\_69</code>](#user-content-test-faults-java-test-69) |
| <code>GET:/app/api/assignments/data/project-commit/{projectId}</code> | 1 | Response status 400 not defined for path '/api/assignments/data/project-commit/{projectId}'. | [<code>faults.java#test\_55</code>](#user-content-test-faults-java-test-55) |
| <code>GET:/app/api/credentials/{id}</code> | 1 | Response status 400 not defined for path '/api/credentials/{id}'. | [<code>faults.java#test\_34</code>](#user-content-test-faults-java-test-34) |
| <code>GET:/app/api/credentials/username/{username}</code> | 1 | Response status 400 not defined for path '/api/credentials/username/{username}'. | [<code>faults.java#test\_40</code>](#user-content-test-faults-java-test-40), [<code>faults.java#test\_42</code>](#user-content-test-faults-java-test-42) |
| <code>GET:/app/api/departments/{id}</code> | 1 | Response status 400 not defined for path '/api/departments/{id}'. | [<code>faults.java#test\_27</code>](#user-content-test-faults-java-test-27) |
| <code>GET:/app/api/employees/{id}</code> | 1 | Response status 400 not defined for path '/api/employees/{id}'. | [<code>faults.java#test\_35</code>](#user-content-test-faults-java-test-35) |
| <code>GET:/app/api/employees/data/department/{departmentId}</code> | 1 | Response status 400 not defined for path '/api/employees/data/department/{departmentId}'. | [<code>faults.java#test\_22</code>](#user-content-test-faults-java-test-22) |
| <code>GET:/app/api/employees/data/employee-project-data/{employeeId}</code> | 1 | Response status 400 not defined for path '/api/employees/data/employee-project-data/{employeeId}'. | [<code>faults.java#test\_66</code>](#user-content-test-faults-java-test-66) |
| <code>GET:/app/api/employees/username/{username}</code> | 1 | Response status 400 not defined for path '/api/employees/username/{username}'. | [<code>faults.java#test\_39</code>](#user-content-test-faults-java-test-39) |
| <code>GET:/app/api/locations/{id}</code> | 1 | Response status 400 not defined for path '/api/locations/{id}'. | [<code>faults.java#test\_57</code>](#user-content-test-faults-java-test-57) |
| <code>GET:/app/api/projects/{id}</code> | 1 | Response status 400 not defined for path '/api/projects/{id}'. | [<code>faults.java#test\_36</code>](#user-content-test-faults-java-test-36) |
| <code>POST:/app/api/assignments</code> | 1 | Response status 400 not defined for path '/api/assignments'. | [<code>faults.java#test\_54</code>](#user-content-test-faults-java-test-54), [<code>faults.java#test\_76</code>](#user-content-test-faults-java-test-76), [<code>faults.java#test\_80</code>](#user-content-test-faults-java-test-80) (+5 more) |
| <code>POST:/app/api/assignments/save</code> | 1 | Response status 400 not defined for path '/api/assignments/save'. | [<code>faults.java#test\_78</code>](#user-content-test-faults-java-test-78), [<code>faults.java#test\_98</code>](#user-content-test-faults-java-test-98) |
| <code>POST:/app/api/authenticate</code> | 1 | Response status 400 not defined for path '/api/authenticate'. | [<code>faults.java#test\_47</code>](#user-content-test-faults-java-test-47) |
| <code>POST:/app/api/authenticate/</code> | 1 | Response status 400 not defined for path '/api/authenticate/'. | [<code>faults.java#test\_94</code>](#user-content-test-faults-java-test-94), [<code>faults.java#test\_97</code>](#user-content-test-faults-java-test-97) |
| <code>POST:/app/api/departments/save</code> | 1 | Response status 400 not defined for path '/api/departments/save'. | [<code>faults.java#test\_84</code>](#user-content-test-faults-java-test-84), [<code>faults.java#test\_103</code>](#user-content-test-faults-java-test-103) |
| <code>POST:/app/api/employees</code> | 1 | Response status 400 not defined for path '/api/employees'. | [<code>faults.java#test\_92</code>](#user-content-test-faults-java-test-92) |
| <code>POST:/app/api/employees/save</code> | 1 | Response status 400 not defined for path '/api/employees/save'. | [<code>faults.java#test\_52</code>](#user-content-test-faults-java-test-52), [<code>faults.java#test\_73</code>](#user-content-test-faults-java-test-73) |
| <code>POST:/app/api/locations</code> | 1 | Response status 400 not defined for path '/api/locations'. | [<code>faults.java#test\_75</code>](#user-content-test-faults-java-test-75), [<code>faults.java#test\_93</code>](#user-content-test-faults-java-test-93) |
| <code>POST:/app/api/locations/save</code> | 1 | Response status 400 not defined for path '/api/locations/save'. | [<code>faults.java#test\_43</code>](#user-content-test-faults-java-test-43) |
| <code>POST:/app/api/projects/save</code> | 1 | Response status 400 not defined for path '/api/projects/save'. | [<code>faults.java#test\_20</code>](#user-content-test-faults-java-test-20), [<code>faults.java#test\_60</code>](#user-content-test-faults-java-test-60) |
| <code>PUT:/app/api/assignments</code> | 1 | Response status 400 not defined for path '/api/assignments'. | [<code>faults.java#test\_41</code>](#user-content-test-faults-java-test-41), [<code>faults.java#test\_108</code>](#user-content-test-faults-java-test-108) |
| <code>PUT:/app/api/assignments/update</code> | 1 | Response status 400 not defined for path '/api/assignments/update'. | [<code>faults.java#test\_53</code>](#user-content-test-faults-java-test-53), [<code>faults.java#test\_77</code>](#user-content-test-faults-java-test-77), [<code>faults.java#test\_100</code>](#user-content-test-faults-java-test-100) |
| <code>PUT:/app/api/credentials</code> | 1 | Response status 400 not defined for path '/api/credentials'. | [<code>faults.java#test\_81</code>](#user-content-test-faults-java-test-81) |
| <code>PUT:/app/api/departments</code> | 1 | Response status 400 not defined for path '/api/departments'. | [<code>faults.java#test\_45</code>](#user-content-test-faults-java-test-45), [<code>faults.java#test\_46</code>](#user-content-test-faults-java-test-46), [<code>faults.java#test\_48</code>](#user-content-test-faults-java-test-48) (+1 more) |
| <code>PUT:/app/api/departments/update</code> | 1 | Response status 400 not defined for path '/api/departments/update'. | [<code>faults.java#test\_85</code>](#user-content-test-faults-java-test-85), [<code>faults.java#test\_86</code>](#user-content-test-faults-java-test-86), [<code>faults.java#test\_90</code>](#user-content-test-faults-java-test-90) |
| <code>PUT:/app/api/employees</code> | 1 | Response status 400 not defined for path '/api/employees'. | [<code>faults.java#test\_49</code>](#user-content-test-faults-java-test-49) |
| <code>PUT:/app/api/employees/update</code> | 1 | Response status 400 not defined for path '/api/employees/update'. | [<code>faults.java#test\_50</code>](#user-content-test-faults-java-test-50) |
| <code>PUT:/app/api/locations</code> | 1 | Response status 400 not defined for path '/api/locations'. | [<code>faults.java#test\_14</code>](#user-content-test-faults-java-test-14), [<code>faults.java#test\_102</code>](#user-content-test-faults-java-test-102) |
| <code>PUT:/app/api/locations/update</code> | 1 | Response status 400 not defined for path '/api/locations/update'. | [<code>faults.java#test\_44</code>](#user-content-test-faults-java-test-44), [<code>faults.java#test\_96</code>](#user-content-test-faults-java-test-96) |
| <code>PUT:/app/api/projects</code> | 1 | Response status 400 not defined for path '/api/projects'. | [<code>faults.java#test\_15</code>](#user-content-test-faults-java-test-15), [<code>faults.java#test\_28</code>](#user-content-test-faults-java-test-28), [<code>faults.java#test\_29</code>](#user-content-test-faults-java-test-29) (+3 more) |
| <code>PUT:/app/api/projects/update</code> | 1 | Response status 400 not defined for path '/api/projects/update'. | [<code>faults.java#test\_74</code>](#user-content-test-faults-java-test-74), [<code>faults.java#test\_82</code>](#user-content-test-faults-java-test-82) |

</details>

<a name="wfc-endpoints"></a>

<details>
<summary>Endpoints (67)</summary>

| Endpoint | Responses | Faults | Test cases |
| --- | --- | --- | --- |
| <code>GET:/app/api/assignments</code> | &#x1F7E2; 200 | &#x1F534; F200 &times;192 | 1 |
| <code>GET:/app/api/assignments/</code> | &#x1F7E2; 200 | &#x1F534; F200 &times;192 | 1 |
| <code>GET:/app/api/employees</code> | &#x1F7E2; 200 | &#x1F534; F200 &times;33 | 1 |
| <code>GET:/app/api/employees/</code> | &#x1F7E2; 200 | &#x1F534; F200 &times;33 | 1 |
| <code>GET:/app/api/credentials</code> | &#x1F7E2; 200 | &#x1F534; F200 &times;6 | 2 |
| <code>POST:/app/api/credentials</code> | &#x1F7E2; 200, &#x1F7E0; 400 | &#x1F534; F200 &times;4 | 4 |
| <code>POST:/app/api/credentials/save</code> | &#x1F7E2; 200, &#x1F7E0; 400 | &#x1F534; F200 &times;4 | 2 |
| <code>GET:/app/api/employees/data/manager-project-data/{employeeId}</code> | &#x1F7E2; 200, &#x1F7E0; 400 | &#x1F534; F200 &times;4 | 2 |
| <code>POST:/app/api/departments</code> | &#x1F7E2; 200, &#x1F7E0; 400 | &#x1F534; F200 &times;3 | 4 |
| <code>POST:/app/api/projects</code> | &#x1F7E2; 200, &#x1F7E0; 400 | &#x1F534; F200 &times;3 | 5 |
| <code>GET:/app/api/credentials/</code> | &#x1F7E2; 200 | &#x1F534; F200 &times;2 | 2 |
| <code>PUT:/app/api/credentials/update</code> | &#x1F7E2; 200, &#x1F7E0; 400 | &#x1F534; F200 &times;2 | 2 |
| <code>GET:/app/api/projects</code> | &#x1F7E2; 200 | &#x1F534; F200 &times;2 | 2 |
| <code>POST:/app/api/assignments</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 8 |
| <code>PUT:/app/api/assignments</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 3 |
| <code>GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}/{commitDate}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>GET:/app/api/assignments/data/project-commit/{projectId}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>DELETE:/app/api/assignments/delete/{employeeId}/{projectId}/{commitDate}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>POST:/app/api/assignments/save</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>PUT:/app/api/assignments/update</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 3 |
| <code>GET:/app/api/assignments/{employeeId}/{projectId}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>GET:/app/api/assignments/{employeeId}/{projectId}/{commitDate}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>DELETE:/app/api/assignments/{employeeId}/{projectId}/{commitDate}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>POST:/app/api/authenticate</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>POST:/app/api/authenticate/</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>PUT:/app/api/credentials</code> | &#x1F7E2; 200, &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>DELETE:/app/api/credentials/delete/{id}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>GET:/app/api/credentials/username/{username}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>DELETE:/app/api/credentials/username/{username}</code> | &#x1F7E2; 200, &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>GET:/app/api/credentials/{id}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>DELETE:/app/api/credentials/{id}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>PUT:/app/api/departments</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 4 |
| <code>DELETE:/app/api/departments/delete/{id}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>POST:/app/api/departments/save</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>PUT:/app/api/departments/update</code> | &#x1F7E2; 200, &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 4 |
| <code>GET:/app/api/departments/{id}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>DELETE:/app/api/departments/{id}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>POST:/app/api/employees</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>PUT:/app/api/employees</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>GET:/app/api/employees/data/department/{departmentId}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>GET:/app/api/employees/data/employee-project-data/{employeeId}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>DELETE:/app/api/employees/delete/{id}</code> | &#x1F7E2; 200, &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>POST:/app/api/employees/save</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>PUT:/app/api/employees/update</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>GET:/app/api/employees/username/{username}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>DELETE:/app/api/employees/username/{username}</code> | &#x1F7E2; 200, &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 3 |
| <code>GET:/app/api/employees/{id}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>DELETE:/app/api/employees/{id}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>POST:/app/api/locations</code> | &#x1F7E2; 200, &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 3 |
| <code>PUT:/app/api/locations</code> | &#x1F7E2; 200, &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 3 |
| <code>DELETE:/app/api/locations/delete/{id}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>POST:/app/api/locations/save</code> | &#x1F7E2; 200, &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>PUT:/app/api/locations/update</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>GET:/app/api/locations/{id}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>DELETE:/app/api/locations/{id}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>PUT:/app/api/projects</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 6 |
| <code>DELETE:/app/api/projects/delete/{id}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 1 |
| <code>POST:/app/api/projects/save</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>PUT:/app/api/projects/update</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>GET:/app/api/projects/{id}</code> | &#x1F7E2; 200, &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>DELETE:/app/api/projects/{id}</code> | &#x1F7E0; 400 | &#x1F534; F200 &times;1 | 2 |
| <code>GET:/app/api/departments</code> | &#x1F7E2; 200 | &#x2705; none | 1 |
| <code>GET:/app/api/departments/</code> | &#x1F7E2; 200 | &#x2705; none | 1 |
| <code>GET:/app/api/locations</code> | &#x1F7E2; 200 | &#x2705; none | 2 |
| <code>GET:/app/api/locations/</code> | &#x1F7E2; 200 | &#x2705; none | 1 |
| <code>GET:/app/api/projects/</code> | &#x1F7E2; 200 | &#x2705; none | 1 |

</details>

<a name="wfc-tests"></a>

### Generated tests (127)

Click a test case id in the tables above to jump to its code.

#### faults.java (110)

<a name="test-faults-java-test-0"></a>
<details open>
<summary><b>test_0</b> &middot; F200 &middot; <code>GET:/app/api/credentials/</code></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/credentials/
    * Found 2 potential faults of type-code 200
    */
    @Test @Timeout(60)
    public void test_0() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/credentials/ -> [Path '/collection/14/role'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/credentials/ -> [Path '/collection/14/username'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/credentials/")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(15))
                .body("'collection'[0].'credentialId'", numberMatches(1.0))
                .body("'collection'[0].'username'", containsString("imentouk"))
                .body("'collection'[0].'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[0].'enabled'", equalTo(true))
                .body("'collection'[0].'role'", containsString("ROLE_EMP"))
                .body("'collection'[1].'credentialId'", numberMatches(2.0))
                .body("'collection'[1].'username'", containsString("badridoudi"))
                .body("'collection'[1].'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[1].'enabled'", equalTo(true))
                .body("'collection'[1].'role'", containsString("ROLE_EMP"))
                .body("'collection'[2].'credentialId'", numberMatches(3.0))
                .body("'collection'[2].'username'", containsString("selimhorri"))
                .body("'collection'[2].'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[2].'enabled'", equalTo(true))
                .body("'collection'[2].'role'", containsString("ROLE_EMP"))
                ; // Skipping assertions on the remaining 12 elements. This limit of 3 elements can be increased in the configurations
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-1"></a>
<details open>
<summary><b>test_1</b> &middot; F200 &middot; <code>GET:/app/api/projects</code></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/projects
    * Found 2 potential faults of type-code 200
    */
    @Test @Timeout(60)
    public void test_1() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("PROJECTS", 143L)
                .d("TITLE", "\"b\"")
                .d("STATUS", "\"G4cNxWPAvx\"")
            .and().insertInto("LOCATIONS", 142L)
                .d("ADR", "\"J8uD\"")
                .d("POSTAL_CODE", "\"PCtWRt9fTl_jGFJa\"")
                .d("CITY", "\"PYpR\"")
            .and().insertInto("DEPARTMENTS", 141L)
                .d("DEPARTMENT_NAME", "\"_ggIRn8pCZdpTh7\"")
            .and().insertInto("EMPLOYEES", 140L)
                .d("FIRST_NAME", "\"4SIYyQN\"")
                .d("LAST_NAME", "\"Jf\"")
                .d("EMAIL", "\"UKs@sd.XAe\"")
                .d("PHONE", "\"p\"")
                .d("JOB", "\"r\"")
                .d("SALARY", "0.6060128345707113")
            .and().insertInto("LOCATIONS", 139L)
                .d("ADR", "\"IzLSuitVf8s8Fk3\"")
                .d("POSTAL_CODE", "\"zSj2\"")
                .d("CITY", "\"20c\"")
            .and().insertInto("DEPARTMENTS", 138L)
                .d("DEPARTMENT_NAME", "\"PKyExGenGGWaJ\"")
            .and().insertInto("EMPLOYEES", 137L)
                .d("FIRST_NAME", "\"x3b6rVD7esITb\"")
                .d("LAST_NAME", "\"gIf\"")
                .d("EMAIL", "\"Fv@h.DHHg\"")
                .d("PHONE", "\"GjlJrEDdeg\"")
                .d("JOB", "\"lcoeYTmySWh\"")
                .d("SALARY", "0.23306002734306475")
            .and().insertInto("LOCATIONS", 136L)
                .d("ADR", "\"1\"")
                .d("POSTAL_CODE", "\"qVDP2ECm3HglIUI\"")
                .d("CITY", "\"N7yqqMOTT\"")
            .and().insertInto("DEPARTMENTS", 135L)
                .d("DEPARTMENT_NAME", "\"0shXKRn\"")
            .and().insertInto("EMPLOYEES", 134L)
                .d("FIRST_NAME", "\"q8FFL8Blw5U\"")
                .d("LAST_NAME", "\"a\"")
                .d("EMAIL", "\"HTb@q.ZR\"")
                .d("PHONE", "\"Z9oGzZ\"")
                .d("JOB", "\"9j\"")
                .d("SALARY", "0.6189236806865404")
            .and().insertInto("ASSIGNMENTS", 133L)
                .d("EMPLOYEE_ID", "12")
                .d("PROJECT_ID", "9")
                .d("COMMIT_DATE", "\"2071-10-13 09:24:55\"")
                .d("COMMIT_EMP_DESC", "\"0746OBdn1\"")
                .d("COMMIT_MGR_DESC", "NULL")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/projects -> [Path '/collection/9/endDate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/projects -> [Path '/collection/9/startDate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/projects")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(10))
                .body("'collection'[0].'projectId'", numberMatches(1.0))
                .body("'collection'[0].'title'", containsString("TRANSBSCS"))
                .body("'collection'[0].'startDate'", containsString("28-09-2020"))
                .body("'collection'[0].'endDate'", containsString("04-11-2020"))
                .body("'collection'[0].'status'", containsString("COMPLETED"))
                .body("'collection'[1].'projectId'", numberMatches(2.0))
                .body("'collection'[1].'title'", containsString("SYNCH_BSCS_IMX"))
                .body("'collection'[1].'startDate'", containsString("26-11-2020"))
                .body("'collection'[1].'endDate'", containsString("25-03-2021"))
                .body("'collection'[1].'status'", containsString("IN_PROGRESS"))
                .body("'collection'[2].'projectId'", numberMatches(3.0))
                .body("'collection'[2].'title'", containsString("TASYI9A LILVIRANDA"))
                .body("'collection'[2].'startDate'", containsString("26-11-2020"))
                .body("'collection'[2].'endDate'", containsString("26-11-2020"))
                .body("'collection'[2].'status'", containsString("COMPLETED"))
                ; // Skipping assertions on the remaining 7 elements. This limit of 3 elements can be increased in the configurations
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-2"></a>
<details open>
<summary><b>test_2</b> &middot; F200 &middot; <code>GET:/app/api/projects</code></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/projects
    * Found 2 potential faults of type-code 200
    */
    @Test @Timeout(60)
    public void test_2() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("PROJECTS", 143L)
                .d("TITLE", "\"b\"")
                .d("STATUS", "\"G4cNxWPAvx\"")
            .and().insertInto("LOCATIONS", 142L)
                .d("ADR", "\"J8uD\"")
                .d("POSTAL_CODE", "\"PCtWRt9fTl_jGFJa\"")
                .d("CITY", "\"PYpR\"")
            .and().insertInto("DEPARTMENTS", 141L)
                .d("DEPARTMENT_NAME", "\"_ggIRn8pCZdpTh7\"")
            .and().insertInto("EMPLOYEES", 140L)
                .d("FIRST_NAME", "\"4SIYyQN\"")
                .d("LAST_NAME", "\"Jf\"")
                .d("EMAIL", "\"UKs@sd.XAe\"")
                .d("PHONE", "\"p\"")
                .d("JOB", "\"r\"")
                .d("SALARY", "0.6060128345707113")
            .and().insertInto("LOCATIONS", 139L)
                .d("ADR", "\"IzLSuitVf8s8Fk3\"")
                .d("POSTAL_CODE", "\"zSj2\"")
                .d("CITY", "\"20c\"")
            .and().insertInto("DEPARTMENTS", 138L)
                .d("DEPARTMENT_NAME", "\"PKyExGenGGWaJ\"")
            .and().insertInto("EMPLOYEES", 137L)
                .d("FIRST_NAME", "\"x3b6rVD7esITb\"")
                .d("LAST_NAME", "\"gIf\"")
                .d("EMAIL", "\"Fv@h.DHHg\"")
                .d("PHONE", "\"GjlJrEDdeg\"")
                .d("JOB", "\"lcoeYTmySWh\"")
                .d("SALARY", "0.23306002734306475")
            .and().insertInto("LOCATIONS", 136L)
                .d("ADR", "\"1\"")
                .d("POSTAL_CODE", "\"qVDP2ECm3HglIUI\"")
                .d("CITY", "\"N7yqqMOTT\"")
            .and().insertInto("DEPARTMENTS", 135L)
                .d("DEPARTMENT_NAME", "\"0shXKRn\"")
            .and().insertInto("EMPLOYEES", 134L)
                .d("FIRST_NAME", "\"q8FFL8Blw5U\"")
                .d("LAST_NAME", "\"a\"")
                .d("EMAIL", "\"HTb@q.ZR\"")
                .d("PHONE", "\"Z9oGzZ\"")
                .d("JOB", "\"9j\"")
                .d("SALARY", "0.6189236806865404")
            .and().insertInto("ASSIGNMENTS", 133L)
                .d("EMPLOYEE_ID", "12")
                .d("PROJECT_ID", "9")
                .d("COMMIT_DATE", "\"2071-10-13 09:24:55\"")
                .d("COMMIT_EMP_DESC", "\"0746OBdn1\"")
                .d("COMMIT_MGR_DESC", "NULL")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/projects -> [Path '/collection/9/endDate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/projects -> [Path '/collection/9/startDate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/projects?" + 
                    "password=g6BKahBUdL4eVi7y&" + 
                    "username=wa")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(10))
                .body("'collection'[0].'projectId'", numberMatches(1.0))
                .body("'collection'[0].'title'", containsString("TRANSBSCS"))
                .body("'collection'[0].'startDate'", containsString("28-09-2020"))
                .body("'collection'[0].'endDate'", containsString("04-11-2020"))
                .body("'collection'[0].'status'", containsString("COMPLETED"))
                .body("'collection'[1].'projectId'", numberMatches(2.0))
                .body("'collection'[1].'title'", containsString("SYNCH_BSCS_IMX"))
                .body("'collection'[1].'startDate'", containsString("26-11-2020"))
                .body("'collection'[1].'endDate'", containsString("25-03-2021"))
                .body("'collection'[1].'status'", containsString("IN_PROGRESS"))
                .body("'collection'[2].'projectId'", numberMatches(3.0))
                .body("'collection'[2].'title'", containsString("TASYI9A LILVIRANDA"))
                .body("'collection'[2].'startDate'", containsString("26-11-2020"))
                .body("'collection'[2].'endDate'", containsString("26-11-2020"))
                .body("'collection'[2].'status'", containsString("COMPLETED"))
                ; // Skipping assertions on the remaining 7 elements. This limit of 3 elements can be increased in the configurations
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-3"></a>
<details open>
<summary><b>test_3</b> &middot; F200 &middot; <code>POST:/app/api/departments</code></summary>

```java
    /**
    * Calls:
    * (200) POST:/app/api/departments
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_3() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/departments -> [Path '/location/postalCode'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .contentType("application/json")
                .body(" { " + 
                    " \"departmentName\": \"Billing\", " + 
                    " \"location\": { " + 
                    " \"adr\": \"EnvNyIV4cb\", " + 
                    " \"city\": \"_EM_99_XYZ_\", " + 
                    " \"locationId\": 2 " + 
                    " } " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/departments?EMextraParam123=42")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'departmentId'", numberMatches(7.0))
                .body("'departmentName'", containsString("Billing"))
                .body("'location'.'locationId'", numberMatches(2.0))
                .body("'location'.'adr'", containsString("EnvNyIV4cb"))
                .body("'location'.'postalCode'", nullValue())
                .body("'location'.'city'", containsString("_EM_99_XYZ_"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-4"></a>
<details open>
<summary><b>test_4</b> &middot; F200 &middot; <code>POST:/app/api/credentials/save</code></summary>

```java
    /**
    * Calls:
    * (200) POST:/app/api/credentials/save
    * Found 3 potential faults of type-code 200
    */
    @Test @Timeout(60)
    public void test_4() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/credentials/save -> [Path '/password'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/credentials/save -> [Path '/role'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/credentials/save -> [Path '/username'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"enabled\": true " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/credentials/save")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'credentialId'", numberMatches(16.0))
                .body("'username'", nullValue())
                .body("'password'", nullValue())
                .body("'enabled'", equalTo(true))
                .body("'role'", nullValue());
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-5"></a>
<details open>
<summary><b>test_5</b> &middot; F200 &middot; <code>GET:/app/api/employees/data/manager-project-data/{employeeId}</code></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/employees/data/manager-project-data/{employeeId}
    * Found 3 potential faults of type-code 200
    */
    @Test @Timeout(60)
    public void test_5() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/data/manager-project-data/{employeeId} -> [Path '/collection/0/title'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/data/manager-project-data/{employeeId} -> [Path '/collection/1/title'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/data/manager-project-data/{employeeId} -> [Path '/collection/2/title'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .get(baseUrlOfSut + "/app/api/employees/data/manager-project-data/5")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(3))
                .body("'collection'[0].'status'", containsString("NOT_STARTED"))
                .body("'collection'[0].'title'", nullValue())
                .body("'collection'[0].'startDate'", containsString("2021-01-29"))
                .body("'collection'[0].'endDate'", containsString("2021-04-30"))
                .body("'collection'[0].'projectId'", numberMatches(4.0))
                .body("'collection'[1].'status'", containsString("IN_PROGRESS"))
                .body("'collection'[1].'title'", nullValue())
                .body("'collection'[1].'startDate'", containsString("2020-11-02"))
                .body("'collection'[1].'endDate'", containsString("2021-05-01"))
                .body("'collection'[1].'projectId'", numberMatches(8.0))
                .body("'collection'[2].'status'", containsString("IN_PROGRESS"))
                .body("'collection'[2].'title'", nullValue())
                .body("'collection'[2].'startDate'", containsString("2020-06-01"))
                .body("'collection'[2].'endDate'", containsString("2021-03-02"))
                .body("'collection'[2].'projectId'", numberMatches(9.0));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-6"></a>
<details open>
<summary><b>test_6</b> &middot; F200 &middot; <code>POST:/app/api/credentials</code></summary>

```java
    /**
    * Calls:
    * (200) POST:/app/api/credentials
    * Found 2 potential faults of type-code 200
    */
    @Test @Timeout(60)
    public void test_6() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/credentials -> [Path '/role'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/credentials -> [Path '/username'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"credentialId\": 344, " + 
                    " \"enabled\": false, " + 
                    " \"password\": \"$2a$10$P0oYDJiBYpHBpaRZ65r/w.nprqp.LU1F6Lxr4z9fOcchEMlvCBjvq\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/credentials")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'credentialId'", numberMatches(18.0))
                .body("'username'", nullValue())
                .body("'password'", containsString("$2a$10$P0oYDJiBYpHBpaRZ65r/w.nprqp.LU1F6Lxr4z9fOcchEMlvCBjvq"))
                .body("'enabled'", equalTo(false))
                .body("'role'", nullValue());
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-7"></a>
<details open>
<summary><b>test_7</b> &middot; F200 &middot; <code>POST:/app/api/credentials</code></summary>

```java
    /**
    * Calls:
    * (200) POST:/app/api/credentials
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_7() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/credentials -> [Path '/password'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" { " + 
                    " \"credentialId\": 20, " + 
                    " \"enabled\": false, " + 
                    " \"role\": \"IsyAMnRlC\", " + 
                    " \"username\": \"TFLe2toPC\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/credentials")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'credentialId'", numberMatches(15.0))
                .body("'username'", containsString("TFLe2toPC"))
                .body("'password'", nullValue())
                .body("'enabled'", equalTo(false))
                .body("'role'", containsString("IsyAMnRlC"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-8"></a>
<details open>
<summary><b>test_8</b> &middot; F200 &middot; <code>PUT:/app/api/credentials/update</code></summary>

```java
    /**
    * Calls:
    * (200) PUT:/app/api/credentials/update
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_8() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/credentials/update -> [Path '/username'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"enabled\": true, " + 
                    " \"password\": \"kdD2FySGiB6XGLxL\", " + 
                    " \"role\": \"ZGixuplV\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/credentials/update")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'credentialId'", numberMatches(17.0))
                .body("'username'", nullValue())
                .body("'password'", containsString("$2a$10$L9/pVck.N0UUzP.FvszBQeCC6uzXlHHcZoyHxO.Y7jK5yT.VnMmP6"))
                .body("'enabled'", equalTo(true))
                .body("'role'", containsString("ZGixuplV"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-9"></a>
<details open>
<summary><b>test_9</b> &middot; F200 &middot; <code>POST:/app/api/departments</code></summary>

```java
    /**
    * Calls:
    * (200) POST:/app/api/departments
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_9() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/departments -> [Path '/location/adr'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" { " + 
                    " \"departmentName\": \"RMc9xpuA\", " + 
                    " \"location\": { " + 
                    " \"city\": \"T8j3egl\", " + 
                    " \"locationId\": 2, " + 
                    " \"postalCode\": \"xc9NPDxyIOXD7OE\" " + 
                    " } " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/departments")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'departmentId'", numberMatches(1.0))
                .body("'departmentName'", containsString("RMc9xpuA"))
                .body("'location'.'locationId'", numberMatches(2.0))
                .body("'location'.'adr'", nullValue())
                .body("'location'.'postalCode'", containsString("xc9NPDxyIOXD7OE"))
                .body("'location'.'city'", containsString("T8j3egl"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-10"></a>
<details open>
<summary><b>test_10</b> &middot; F200 &middot; <code>POST:/app/api/projects</code></summary>

```java
    /**
    * Calls:
    * (200) POST:/app/api/projects
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_10() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/projects -> [Path '/startDate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .contentType("application/json")
                .body(" { " + 
                    " \"endDate\": \"01-05-2021\", " + 
                    " \"projectId\": 9, " + 
                    " \"status\": \"G8\", " + 
                    " \"title\": \"1V3eM\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/projects")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'projectId'", numberMatches(9.0))
                .body("'title'", containsString("1V3eM"))
                .body("'startDate'", nullValue())
                .body("'endDate'", containsString("01-05-2021"))
                .body("'status'", containsString("G8"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-11"></a>
<details open>
<summary><b>test_11</b> &middot; F200 &middot; <code>GET:/app/api/credentials</code> (+1 more)</summary>

```java
    /**
    * Calls:
    * 1 - (400) POST:/app/api/credentials
    * 2 - (200) GET:/app/api/credentials
    * Found 7 potential faults of type-code 200
    */
    @Test @Timeout(60)
    public void test_11() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/credentials -> Response status 400 not defined for path '/api/credentials'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .contentType("application/json")
                .body(" { " + 
                    " \"credentialId\": 3, " + 
                    " \"role\": \"pEgKhuzkX\", " + 
                    " \"username\": \"_EM_407_XYZ_\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/credentials")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("could not execute statement; SQL [n/a]; constraint [null]; nested exception is org.hibernate.exception.ConstraintViolationException: could not execute statement"))
                .body("'status'", containsString("BAD_REQUEST"));
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/credentials -> [Path '/collection/14/password'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/credentials -> [Path '/collection/14/role'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/credentials -> [Path '/collection/14/username'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/credentials -> [Path '/collection/15/username'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/credentials -> [Path '/collection/16/role'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/credentials -> [Path '/collection/16/username'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/credentials")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(17))
                .body("'collection'[0].'credentialId'", numberMatches(1.0))
                .body("'collection'[0].'username'", containsString("imentouk"))
                .body("'collection'[0].'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[0].'enabled'", equalTo(true))
                .body("'collection'[0].'role'", containsString("ROLE_EMP"))
                .body("'collection'[1].'credentialId'", numberMatches(2.0))
                .body("'collection'[1].'username'", containsString("badridoudi"))
                .body("'collection'[1].'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[1].'enabled'", equalTo(true))
                .body("'collection'[1].'role'", containsString("ROLE_EMP"))
                .body("'collection'[2].'credentialId'", numberMatches(3.0))
                .body("'collection'[2].'username'", containsString("selimhorri"))
                .body("'collection'[2].'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[2].'enabled'", equalTo(true))
                .body("'collection'[2].'role'", containsString("ROLE_EMP"))
                ; // Skipping assertions on the remaining 14 elements. This limit of 3 elements can be increased in the configurations
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-12"></a>
<details open>
<summary><b>test_12</b> &middot; F200 &middot; <code>GET:/app/api/employees</code></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/employees
    * Found 33 potential faults of type-code 200
    */
    @Test @Timeout(60)
    public void test_12() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/0/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/0/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/1/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/1/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/2/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/2/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/3/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/3/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/4/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/4/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/5/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/5/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/6/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/6/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/6/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/7/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/7/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/8/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/8/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/9/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/9/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/9/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/10/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/10/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/10/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/11/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/11/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/12/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/12/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/12/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/13/department'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/13/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees -> [Path '/collection/13/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "42")
                .get(baseUrlOfSut + "/app/api/employees")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(14))
                .body("'collection'[0].'employeeId'", numberMatches(1.0))
                .body("'collection'[0].'firstName'", containsString("Selim"))
                .body("'collection'[0].'lastName'", containsString("Horri"))
                .body("'collection'[0].'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[0].'phone'", containsString("22125144"))
                .body("'collection'[0].'hiredate'", containsString("15-04-2019"))
                .body("'collection'[0].'job'", containsString("Billing"))
                .body("'collection'[0].'salary'", numberMatches(5000.0))
                .body("'collection'[0].'manager'.'employeeId'", numberMatches(4.0))
                .body("'collection'[0].'manager'.'firstName'", containsString("Soumaya"))
                .body("'collection'[0].'manager'.'lastName'", containsString("Hajjem"))
                .body("'collection'[0].'manager'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[0].'manager'.'phone'", containsString("22125144"))
                .body("'collection'[0].'manager'.'hiredate'", nullValue())
                .body("'collection'[0].'manager'.'job'", containsString("Chef service Billing"))
                .body("'collection'[0].'manager'.'salary'", numberMatches(6000.0))
                .body("'collection'[0].'manager'.'manager'", nullValue())
                .body("'collection'[0].'manager'.'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[0].'manager'.'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[0].'manager'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[0].'manager'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[0].'manager'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[0].'manager'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[0].'manager'.'credential'.'credentialId'", numberMatches(5.0))
                .body("'collection'[0].'manager'.'credential'.'username'", containsString("soumayahajjem"))
                .body("'collection'[0].'manager'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[0].'manager'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[0].'manager'.'credential'.'role'", containsString("ROLE_MGR"))
                .body("'collection'[0].'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[0].'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[0].'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[0].'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[0].'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[0].'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[0].'credential'.'credentialId'", numberMatches(3.0))
                .body("'collection'[0].'credential'.'username'", containsString("selimhorri"))
                .body("'collection'[0].'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[0].'credential'.'enabled'", equalTo(true))
                .body("'collection'[0].'credential'.'role'", containsString("ROLE_EMP"))
                .body("'collection'[1].'employeeId'", numberMatches(2.0))
                .body("'collection'[1].'firstName'", containsString("Badr"))
                .body("'collection'[1].'lastName'", containsString("Idoudi"))
                .body("'collection'[1].'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[1].'phone'", containsString("22125144"))
                .body("'collection'[1].'hiredate'", containsString("15-04-2019"))
                .body("'collection'[1].'job'", containsString("Digital"))
                .body("'collection'[1].'salary'", numberMatches(5000.0))
                .body("'collection'[1].'manager'.'employeeId'", numberMatches(9.0))
                .body("'collection'[1].'manager'.'firstName'", containsString("John"))
                .body("'collection'[1].'manager'.'lastName'", containsString("Doe"))
                .body("'collection'[1].'manager'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[1].'manager'.'phone'", containsString("22125144"))
                .body("'collection'[1].'manager'.'hiredate'", nullValue())
                .body("'collection'[1].'manager'.'job'", containsString("Chef service digital"))
                .body("'collection'[1].'manager'.'salary'", numberMatches(6000.0))
                .body("'collection'[1].'manager'.'manager'", nullValue())
                .body("'collection'[1].'manager'.'department'.'departmentId'", numberMatches(5.0))
                .body("'collection'[1].'manager'.'department'.'departmentName'", containsString("Digital"))
                .body("'collection'[1].'manager'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[1].'manager'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[1].'manager'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[1].'manager'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[1].'manager'.'credential'.'credentialId'", numberMatches(7.0))
                .body("'collection'[1].'manager'.'credential'.'username'", containsString("johndoe"))
                .body("'collection'[1].'manager'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[1].'manager'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[1].'manager'.'credential'.'role'", containsString("ROLE_MGR"))
                .body("'collection'[1].'department'.'departmentId'", numberMatches(5.0))
                .body("'collection'[1].'department'.'departmentName'", containsString("Digital"))
                .body("'collection'[1].'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[1].'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[1].'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[1].'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[1].'credential'.'credentialId'", numberMatches(2.0))
                .body("'collection'[1].'credential'.'username'", containsString("badridoudi"))
                .body("'collection'[1].'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[1].'credential'.'enabled'", equalTo(true))
                .body("'collection'[1].'credential'.'role'", containsString("ROLE_EMP"))
                .body("'collection'[2].'employeeId'", numberMatches(3.0))
                .body("'collection'[2].'firstName'", containsString("Imen"))
                .body("'collection'[2].'lastName'", containsString("Touk"))
                .body("'collection'[2].'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[2].'phone'", containsString("22125144"))
                .body("'collection'[2].'hiredate'", containsString("15-04-2019"))
                .body("'collection'[2].'job'", containsString("Data Warehouse"))
                .body("'collection'[2].'salary'", numberMatches(5000.0))
                .body("'collection'[2].'manager'.'employeeId'", numberMatches(5.0))
                .body("'collection'[2].'manager'.'firstName'", containsString("Nour"))
                .body("'collection'[2].'manager'.'lastName'", containsString("Larguech"))
                .body("'collection'[2].'manager'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[2].'manager'.'phone'", containsString("22125144"))
                .body("'collection'[2].'manager'.'hiredate'", nullValue())
                .body("'collection'[2].'manager'.'job'", containsString("Chef service Data Warehouse"))
                .body("'collection'[2].'manager'.'salary'", numberMatches(6000.0))
                .body("'collection'[2].'manager'.'manager'", nullValue())
                .body("'collection'[2].'manager'.'department'.'departmentId'", numberMatches(4.0))
                .body("'collection'[2].'manager'.'department'.'departmentName'", containsString("DWH"))
                .body("'collection'[2].'manager'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[2].'manager'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[2].'manager'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[2].'manager'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[2].'manager'.'credential'.'credentialId'", numberMatches(6.0))
                .body("'collection'[2].'manager'.'credential'.'username'", containsString("nourlarguech"))
                .body("'collection'[2].'manager'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[2].'manager'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[2].'manager'.'credential'.'role'", containsString("ROLE_MGR"))
                .body("'collection'[2].'department'.'departmentId'", numberMatches(4.0))
                .body("'collection'[2].'department'.'departmentName'", containsString("DWH"))
                .body("'collection'[2].'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[2].'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[2].'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[2].'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[2].'credential'.'credentialId'", numberMatches(1.0))
                .body("'collection'[2].'credential'.'username'", containsString("imentouk"))
                .body("'collection'[2].'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[2].'credential'.'enabled'", equalTo(true))
                .body("'collection'[2].'credential'.'role'", containsString("ROLE_EMP"))
                ; // Skipping assertions on the remaining 11 elements. This limit of 3 elements can be increased in the configurations
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-13"></a>
<details open>
<summary><b>test_13</b> &middot; F200 &middot; <code>GET:/app/api/employees/</code></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/employees/
    * Found 33 potential faults of type-code 200
    */
    @Test @Timeout(60)
    public void test_13() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/0/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/0/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/1/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/1/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/2/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/2/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/3/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/3/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/4/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/4/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/5/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/5/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/6/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/6/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/6/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/7/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/7/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/8/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/8/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/9/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/9/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/9/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/10/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/10/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/10/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/11/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/11/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/12/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/12/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/12/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/13/department'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/13/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/ -> [Path '/collection/13/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/employees/?EMextraParam123=42")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(14))
                .body("'collection'[0].'employeeId'", numberMatches(1.0))
                .body("'collection'[0].'firstName'", containsString("Selim"))
                .body("'collection'[0].'lastName'", containsString("Horri"))
                .body("'collection'[0].'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[0].'phone'", containsString("22125144"))
                .body("'collection'[0].'hiredate'", containsString("15-04-2019"))
                .body("'collection'[0].'job'", containsString("Billing"))
                .body("'collection'[0].'salary'", numberMatches(5000.0))
                .body("'collection'[0].'manager'.'employeeId'", numberMatches(4.0))
                .body("'collection'[0].'manager'.'firstName'", containsString("Soumaya"))
                .body("'collection'[0].'manager'.'lastName'", containsString("Hajjem"))
                .body("'collection'[0].'manager'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[0].'manager'.'phone'", containsString("22125144"))
                .body("'collection'[0].'manager'.'hiredate'", nullValue())
                .body("'collection'[0].'manager'.'job'", containsString("Chef service Billing"))
                .body("'collection'[0].'manager'.'salary'", numberMatches(6000.0))
                .body("'collection'[0].'manager'.'manager'", nullValue())
                .body("'collection'[0].'manager'.'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[0].'manager'.'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[0].'manager'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[0].'manager'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[0].'manager'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[0].'manager'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[0].'manager'.'credential'.'credentialId'", numberMatches(5.0))
                .body("'collection'[0].'manager'.'credential'.'username'", containsString("soumayahajjem"))
                .body("'collection'[0].'manager'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[0].'manager'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[0].'manager'.'credential'.'role'", containsString("ROLE_MGR"))
                .body("'collection'[0].'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[0].'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[0].'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[0].'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[0].'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[0].'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[0].'credential'.'credentialId'", numberMatches(3.0))
                .body("'collection'[0].'credential'.'username'", containsString("selimhorri"))
                .body("'collection'[0].'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[0].'credential'.'enabled'", equalTo(true))
                .body("'collection'[0].'credential'.'role'", containsString("ROLE_EMP"))
                .body("'collection'[1].'employeeId'", numberMatches(2.0))
                .body("'collection'[1].'firstName'", containsString("Badr"))
                .body("'collection'[1].'lastName'", containsString("Idoudi"))
                .body("'collection'[1].'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[1].'phone'", containsString("22125144"))
                .body("'collection'[1].'hiredate'", containsString("15-04-2019"))
                .body("'collection'[1].'job'", containsString("Digital"))
                .body("'collection'[1].'salary'", numberMatches(5000.0))
                .body("'collection'[1].'manager'.'employeeId'", numberMatches(9.0))
                .body("'collection'[1].'manager'.'firstName'", containsString("John"))
                .body("'collection'[1].'manager'.'lastName'", containsString("Doe"))
                .body("'collection'[1].'manager'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[1].'manager'.'phone'", containsString("22125144"))
                .body("'collection'[1].'manager'.'hiredate'", nullValue())
                .body("'collection'[1].'manager'.'job'", containsString("Chef service digital"))
                .body("'collection'[1].'manager'.'salary'", numberMatches(6000.0))
                .body("'collection'[1].'manager'.'manager'", nullValue())
                .body("'collection'[1].'manager'.'department'.'departmentId'", numberMatches(5.0))
                .body("'collection'[1].'manager'.'department'.'departmentName'", containsString("Digital"))
                .body("'collection'[1].'manager'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[1].'manager'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[1].'manager'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[1].'manager'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[1].'manager'.'credential'.'credentialId'", numberMatches(7.0))
                .body("'collection'[1].'manager'.'credential'.'username'", containsString("johndoe"))
                .body("'collection'[1].'manager'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[1].'manager'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[1].'manager'.'credential'.'role'", containsString("ROLE_MGR"))
                .body("'collection'[1].'department'.'departmentId'", numberMatches(5.0))
                .body("'collection'[1].'department'.'departmentName'", containsString("Digital"))
                .body("'collection'[1].'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[1].'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[1].'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[1].'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[1].'credential'.'credentialId'", numberMatches(2.0))
                .body("'collection'[1].'credential'.'username'", containsString("badridoudi"))
                .body("'collection'[1].'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[1].'credential'.'enabled'", equalTo(true))
                .body("'collection'[1].'credential'.'role'", containsString("ROLE_EMP"))
                .body("'collection'[2].'employeeId'", numberMatches(3.0))
                .body("'collection'[2].'firstName'", containsString("Imen"))
                .body("'collection'[2].'lastName'", containsString("Touk"))
                .body("'collection'[2].'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[2].'phone'", containsString("22125144"))
                .body("'collection'[2].'hiredate'", containsString("15-04-2019"))
                .body("'collection'[2].'job'", containsString("Data Warehouse"))
                .body("'collection'[2].'salary'", numberMatches(5000.0))
                .body("'collection'[2].'manager'.'employeeId'", numberMatches(5.0))
                .body("'collection'[2].'manager'.'firstName'", containsString("Nour"))
                .body("'collection'[2].'manager'.'lastName'", containsString("Larguech"))
                .body("'collection'[2].'manager'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[2].'manager'.'phone'", containsString("22125144"))
                .body("'collection'[2].'manager'.'hiredate'", nullValue())
                .body("'collection'[2].'manager'.'job'", containsString("Chef service Data Warehouse"))
                .body("'collection'[2].'manager'.'salary'", numberMatches(6000.0))
                .body("'collection'[2].'manager'.'manager'", nullValue())
                .body("'collection'[2].'manager'.'department'.'departmentId'", numberMatches(4.0))
                .body("'collection'[2].'manager'.'department'.'departmentName'", containsString("DWH"))
                .body("'collection'[2].'manager'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[2].'manager'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[2].'manager'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[2].'manager'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[2].'manager'.'credential'.'credentialId'", numberMatches(6.0))
                .body("'collection'[2].'manager'.'credential'.'username'", containsString("nourlarguech"))
                .body("'collection'[2].'manager'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[2].'manager'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[2].'manager'.'credential'.'role'", containsString("ROLE_MGR"))
                .body("'collection'[2].'department'.'departmentId'", numberMatches(4.0))
                .body("'collection'[2].'department'.'departmentName'", containsString("DWH"))
                .body("'collection'[2].'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[2].'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[2].'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[2].'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[2].'credential'.'credentialId'", numberMatches(1.0))
                .body("'collection'[2].'credential'.'username'", containsString("imentouk"))
                .body("'collection'[2].'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[2].'credential'.'enabled'", equalTo(true))
                .body("'collection'[2].'credential'.'role'", containsString("ROLE_EMP"))
                ; // Skipping assertions on the remaining 11 elements. This limit of 3 elements can be increased in the configurations
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-14"></a>
<details open>
<summary><b>test_14</b> &middot; F200 &middot; <code>PUT:/app/api/locations</code></summary>

```java
    /**
    * Calls:
    * 1 - (400) PUT:/app/api/locations
    * 2 - (200) POST:/app/api/locations
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_14() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/locations -> Response status 400 not defined for path '/api/locations'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"adr\": \"WirX\", " + 
                    " \"postalCode\": \"Z\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/locations")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Validation failed for classes [com.pfa.app.model.entity.Location] during persist time for groups [javax.validation.groups.Default, ]\nList of constraint violations:[\n\tConstraintViolationImpl{interpolatedMessage='*Must Not blank**', propertyPath=city, rootBeanClass=class com.pfa.app.model.entity.Location, messageTemplate='*Must Not blank**'}\n]"))
                .body("'status'", containsString("BAD_REQUEST"));
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"adr\": \"WirX\", " + 
                    " \"city\": \"_FxO6dv6KTq\", " + 
                    " \"postalCode\": \"Z\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/locations")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'locationId'", numberMatches(3.0))
                .body("'adr'", containsString("WirX"))
                .body("'postalCode'", containsString("Z"))
                .body("'city'", containsString("_FxO6dv6KTq"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-15"></a>
<details open>
<summary><b>test_15</b> &middot; F200 &middot; <code>POST:/app/api/projects</code> (+1 more)</summary>

```java
    /**
    * Calls:
    * 1 - (200) POST:/app/api/projects
    * 2 - (400) PUT:/app/api/projects
    * Found 3 potential faults of type-code 200
    * Using 1 example:
    *   dd-MM-yyyy
    */
    @Test @Timeout(60)
    public void test_15() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/projects -> [Path '/endDate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/projects -> [Path '/startDate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"status\": \"x03Fs\", " + 
                    " \"title\": \"pkZsE6JebHQ\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/projects")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'projectId'", numberMatches(10.0))
                .body("'title'", containsString("pkZsE6JebHQ"))
                .body("'startDate'", nullValue())
                .body("'endDate'", nullValue())
                .body("'status'", containsString("x03Fs"));
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/projects -> Response status 400 not defined for path '/api/projects'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"endDate\": \"dd-MM-yyyy\", " + 
                    " \"startDate\": \"dd-MM-yyyy\", " + 
                    " \"title\": \"pkZsE6JebHQ\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/projects")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 12] (through reference chain: com.pfa.app.model.entity.Project[\"endDate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-16"></a>
<details open>
<summary><b>test_16</b> &middot; F200 &middot; <code>GET:/app/api/assignments</code></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/assignments
    * Found 192 potential faults of type-code 200
    */
    @Test @Timeout(60)
    public void test_16() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/0/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/0/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/0/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/1/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/1/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/2/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/2/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/2/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/3/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/3/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/3/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/4/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/4/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/4/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/5/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/5/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/5/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/6/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/6/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/6/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/7/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/7/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/8/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/8/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/8/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/9/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/9/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/9/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/10/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/10/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/10/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/11/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/11/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/11/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/12/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/12/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/12/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/13/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/13/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/13/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/14/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/14/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/14/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/15/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/15/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/15/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/16/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/16/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/16/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/17/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/17/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/17/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/18/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/18/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/18/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/19/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/19/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/19/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/20/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/20/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/20/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/21/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/21/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/21/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/22/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/22/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/22/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/23/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/23/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/23/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/24/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/24/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/24/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/25/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/25/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/25/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/26/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/26/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/26/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/27/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/27/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/27/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/28/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/28/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/28/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/29/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/29/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/29/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/30/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/30/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/30/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/31/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/31/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/31/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/32/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/32/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/32/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/33/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/33/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/33/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/34/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/34/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/34/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/35/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/35/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/35/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/36/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/36/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/36/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/36/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/37/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/37/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/37/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/37/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/38/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/38/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/38/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/38/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/39/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/39/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/39/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/39/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/40/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/40/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/40/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/40/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/41/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/41/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/41/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/41/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/42/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/42/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/42/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/42/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/43/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/43/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/43/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/43/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/44/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/44/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/44/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/44/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/45/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/45/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/45/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/45/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/46/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/46/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/46/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/46/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/47/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/47/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/47/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/48/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/48/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/48/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/49/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/49/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/49/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/50/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/50/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/50/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/51/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/51/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/51/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/52/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/52/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/52/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/53/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/53/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/53/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/53/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/54/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/54/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/54/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/54/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/55/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/55/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/55/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/55/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/56/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/56/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/56/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/56/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/57/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/57/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/57/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/57/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/58/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/58/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/58/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments -> [Path '/collection/58/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "42")
                .get(baseUrlOfSut + "/app/api/assignments?EMextraParam123=42")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(59))
                .body("'collection'[0].'employeeId'", numberMatches(1.0))
                .body("'collection'[0].'projectId'", numberMatches(1.0))
                .body("'collection'[0].'commitDate'", containsString("26-11-202010:50:09"))
                .body("'collection'[0].'commitEmpDesc'", nullValue())
                .body("'collection'[0].'commitMgrDesc'", containsString("init"))
                .body("'collection'[0].'employee'.'employeeId'", numberMatches(1.0))
                .body("'collection'[0].'employee'.'firstName'", containsString("Selim"))
                .body("'collection'[0].'employee'.'lastName'", containsString("Horri"))
                .body("'collection'[0].'employee'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[0].'employee'.'phone'", containsString("22125144"))
                .body("'collection'[0].'employee'.'hiredate'", containsString("15-04-2019"))
                .body("'collection'[0].'employee'.'job'", containsString("Billing"))
                .body("'collection'[0].'employee'.'salary'", numberMatches(5000.0))
                .body("'collection'[0].'employee'.'manager'.'employeeId'", numberMatches(4.0))
                .body("'collection'[0].'employee'.'manager'.'firstName'", containsString("Soumaya"))
                .body("'collection'[0].'employee'.'manager'.'lastName'", containsString("Hajjem"))
                .body("'collection'[0].'employee'.'manager'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[0].'employee'.'manager'.'phone'", containsString("22125144"))
                .body("'collection'[0].'employee'.'manager'.'hiredate'", nullValue())
                .body("'collection'[0].'employee'.'manager'.'job'", containsString("Chef service Billing"))
                .body("'collection'[0].'employee'.'manager'.'salary'", numberMatches(6000.0))
                .body("'collection'[0].'employee'.'manager'.'manager'", nullValue())
                .body("'collection'[0].'employee'.'manager'.'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[0].'employee'.'manager'.'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[0].'employee'.'manager'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[0].'employee'.'manager'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[0].'employee'.'manager'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[0].'employee'.'manager'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[0].'employee'.'manager'.'credential'.'credentialId'", numberMatches(5.0))
                .body("'collection'[0].'employee'.'manager'.'credential'.'username'", containsString("soumayahajjem"))
                .body("'collection'[0].'employee'.'manager'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[0].'employee'.'manager'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[0].'employee'.'manager'.'credential'.'role'", containsString("ROLE_MGR"))
                .body("'collection'[0].'employee'.'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[0].'employee'.'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[0].'employee'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[0].'employee'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[0].'employee'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[0].'employee'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[0].'employee'.'credential'.'credentialId'", numberMatches(3.0))
                .body("'collection'[0].'employee'.'credential'.'username'", containsString("selimhorri"))
                .body("'collection'[0].'employee'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[0].'employee'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[0].'employee'.'credential'.'role'", containsString("ROLE_EMP"))
                .body("'collection'[0].'project'.'projectId'", numberMatches(1.0))
                .body("'collection'[0].'project'.'title'", containsString("TRANSBSCS"))
                .body("'collection'[0].'project'.'startDate'", containsString("28-09-2020"))
                .body("'collection'[0].'project'.'endDate'", containsString("04-11-2020"))
                .body("'collection'[0].'project'.'status'", containsString("COMPLETED"))
                .body("'collection'[1].'employeeId'", numberMatches(1.0))
                .body("'collection'[1].'projectId'", numberMatches(1.0))
                .body("'collection'[1].'commitDate'", containsString("26-11-202013:14:22"))
                .body("'collection'[1].'commitEmpDesc'", containsString("set up some configs"))
                .body("'collection'[1].'commitMgrDesc'", containsString("you need to implement sec solution"))
                .body("'collection'[1].'employee'.'employeeId'", numberMatches(1.0))
                .body("'collection'[1].'employee'.'firstName'", containsString("Selim"))
                .body("'collection'[1].'employee'.'lastName'", containsString("Horri"))
                .body("'collection'[1].'employee'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[1].'employee'.'phone'", containsString("22125144"))
                .body("'collection'[1].'employee'.'hiredate'", containsString("15-04-2019"))
                .body("'collection'[1].'employee'.'job'", containsString("Billing"))
                .body("'collection'[1].'employee'.'salary'", numberMatches(5000.0))
                .body("'collection'[1].'employee'.'manager'.'employeeId'", numberMatches(4.0))
                .body("'collection'[1].'employee'.'manager'.'firstName'", containsString("Soumaya"))
                .body("'collection'[1].'employee'.'manager'.'lastName'", containsString("Hajjem"))
                .body("'collection'[1].'employee'.'manager'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[1].'employee'.'manager'.'phone'", containsString("22125144"))
                .body("'collection'[1].'employee'.'manager'.'hiredate'", nullValue())
                .body("'collection'[1].'employee'.'manager'.'job'", containsString("Chef service Billing"))
                .body("'collection'[1].'employee'.'manager'.'salary'", numberMatches(6000.0))
                .body("'collection'[1].'employee'.'manager'.'manager'", nullValue())
                .body("'collection'[1].'employee'.'manager'.'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[1].'employee'.'manager'.'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[1].'employee'.'manager'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[1].'employee'.'manager'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[1].'employee'.'manager'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[1].'employee'.'manager'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[1].'employee'.'manager'.'credential'.'credentialId'", numberMatches(5.0))
                .body("'collection'[1].'employee'.'manager'.'credential'.'username'", containsString("soumayahajjem"))
                .body("'collection'[1].'employee'.'manager'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[1].'employee'.'manager'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[1].'employee'.'manager'.'credential'.'role'", containsString("ROLE_MGR"))
                .body("'collection'[1].'employee'.'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[1].'employee'.'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[1].'employee'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[1].'employee'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[1].'employee'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[1].'employee'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[1].'employee'.'credential'.'credentialId'", numberMatches(3.0))
                .body("'collection'[1].'employee'.'credential'.'username'", containsString("selimhorri"))
                .body("'collection'[1].'employee'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[1].'employee'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[1].'employee'.'credential'.'role'", containsString("ROLE_EMP"))
                .body("'collection'[1].'project'.'projectId'", numberMatches(1.0))
                .body("'collection'[1].'project'.'title'", containsString("TRANSBSCS"))
                .body("'collection'[1].'project'.'startDate'", containsString("28-09-2020"))
                .body("'collection'[1].'project'.'endDate'", containsString("04-11-2020"))
                .body("'collection'[1].'project'.'status'", containsString("COMPLETED"))
                .body("'collection'[2].'employeeId'", numberMatches(1.0))
                .body("'collection'[2].'projectId'", numberMatches(1.0))
                .body("'collection'[2].'commitDate'", containsString("12-12-202016:49:42"))
                .body("'collection'[2].'commitEmpDesc'", containsString("implement customer by invoice"))
                .body("'collection'[2].'commitMgrDesc'", nullValue())
                .body("'collection'[2].'employee'.'employeeId'", numberMatches(1.0))
                .body("'collection'[2].'employee'.'firstName'", containsString("Selim"))
                .body("'collection'[2].'employee'.'lastName'", containsString("Horri"))
                .body("'collection'[2].'employee'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[2].'employee'.'phone'", containsString("22125144"))
                .body("'collection'[2].'employee'.'hiredate'", containsString("15-04-2019"))
                .body("'collection'[2].'employee'.'job'", containsString("Billing"))
                .body("'collection'[2].'employee'.'salary'", numberMatches(5000.0))
                .body("'collection'[2].'employee'.'manager'.'employeeId'", numberMatches(4.0))
                .body("'collection'[2].'employee'.'manager'.'firstName'", containsString("Soumaya"))
                .body("'collection'[2].'employee'.'manager'.'lastName'", containsString("Hajjem"))
                .body("'collection'[2].'employee'.'manager'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[2].'employee'.'manager'.'phone'", containsString("22125144"))
                .body("'collection'[2].'employee'.'manager'.'hiredate'", nullValue())
                .body("'collection'[2].'employee'.'manager'.'job'", containsString("Chef service Billing"))
                .body("'collection'[2].'employee'.'manager'.'salary'", numberMatches(6000.0))
                .body("'collection'[2].'employee'.'manager'.'manager'", nullValue())
                .body("'collection'[2].'employee'.'manager'.'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[2].'employee'.'manager'.'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[2].'employee'.'manager'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[2].'employee'.'manager'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[2].'employee'.'manager'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[2].'employee'.'manager'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[2].'employee'.'manager'.'credential'.'credentialId'", numberMatches(5.0))
                .body("'collection'[2].'employee'.'manager'.'credential'.'username'", containsString("soumayahajjem"))
                .body("'collection'[2].'employee'.'manager'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[2].'employee'.'manager'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[2].'employee'.'manager'.'credential'.'role'", containsString("ROLE_MGR"))
                .body("'collection'[2].'employee'.'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[2].'employee'.'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[2].'employee'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[2].'employee'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[2].'employee'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[2].'employee'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[2].'employee'.'credential'.'credentialId'", numberMatches(3.0))
                .body("'collection'[2].'employee'.'credential'.'username'", containsString("selimhorri"))
                .body("'collection'[2].'employee'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[2].'employee'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[2].'employee'.'credential'.'role'", containsString("ROLE_EMP"))
                .body("'collection'[2].'project'.'projectId'", numberMatches(1.0))
                .body("'collection'[2].'project'.'title'", containsString("TRANSBSCS"))
                .body("'collection'[2].'project'.'startDate'", containsString("28-09-2020"))
                .body("'collection'[2].'project'.'endDate'", containsString("04-11-2020"))
                .body("'collection'[2].'project'.'status'", containsString("COMPLETED"))
                ; // Skipping assertions on the remaining 56 elements. This limit of 3 elements can be increased in the configurations
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-17"></a>
<details open>
<summary><b>test_17</b> &middot; F200 &middot; <code>GET:/app/api/assignments/</code></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/assignments/
    * Found 192 potential faults of type-code 200
    */
    @Test @Timeout(60)
    public void test_17() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/0/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/0/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/0/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/1/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/1/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/2/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/2/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/2/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/3/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/3/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/3/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/4/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/4/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/4/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/5/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/5/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/5/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/6/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/6/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/6/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/7/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/7/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/8/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/8/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/8/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/9/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/9/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/9/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/10/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/10/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/10/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/11/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/11/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/11/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/12/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/12/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/12/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/13/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/13/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/13/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/14/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/14/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/14/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/15/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/15/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/15/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/16/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/16/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/16/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/17/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/17/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/17/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/18/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/18/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/18/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/19/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/19/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/19/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/20/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/20/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/20/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/21/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/21/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/21/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/22/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/22/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/22/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/23/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/23/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/23/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/24/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/24/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/24/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/25/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/25/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/25/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/26/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/26/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/26/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/27/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/27/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/27/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/28/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/28/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/28/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/29/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/29/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/29/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/30/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/30/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/30/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/31/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/31/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/31/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/32/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/32/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/32/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/33/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/33/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/33/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/34/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/34/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/34/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/35/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/35/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/35/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/36/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/36/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/36/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/36/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/37/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/37/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/37/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/37/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/38/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/38/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/38/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/38/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/39/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/39/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/39/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/39/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/40/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/40/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/40/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/40/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/41/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/41/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/41/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/41/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/42/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/42/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/42/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/42/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/43/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/43/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/43/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/43/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/44/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/44/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/44/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/44/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/45/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/45/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/45/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/45/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/46/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/46/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/46/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/46/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/47/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/47/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/47/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/48/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/48/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/48/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/49/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/49/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/49/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/50/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/50/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/50/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/51/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/51/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/51/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/52/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/52/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/52/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/53/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/53/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/53/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/53/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/54/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/54/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/54/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/54/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/55/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/55/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/55/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/55/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/56/commitEmpDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/56/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/56/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/56/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/57/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/57/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/57/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/57/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/58/commitMgrDesc'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/58/employee/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/58/employee/manager/hiredate'] Instance type (null) does not match any allowed primitive type (allowed: ["string"])
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/ -> [Path '/collection/58/employee/manager/manager'] Instance type (null) does not match any allowed primitive type (allowed: ["object"])
        given().accept("*/*")
                .header("x-EMextraHeader123", "_EM_52_XYZ_")
                .get(baseUrlOfSut + "/app/api/assignments/")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(59))
                .body("'collection'[0].'employeeId'", numberMatches(1.0))
                .body("'collection'[0].'projectId'", numberMatches(1.0))
                .body("'collection'[0].'commitDate'", containsString("26-11-202010:50:09"))
                .body("'collection'[0].'commitEmpDesc'", nullValue())
                .body("'collection'[0].'commitMgrDesc'", containsString("init"))
                .body("'collection'[0].'employee'.'employeeId'", numberMatches(1.0))
                .body("'collection'[0].'employee'.'firstName'", containsString("Selim"))
                .body("'collection'[0].'employee'.'lastName'", containsString("Horri"))
                .body("'collection'[0].'employee'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[0].'employee'.'phone'", containsString("22125144"))
                .body("'collection'[0].'employee'.'hiredate'", containsString("15-04-2019"))
                .body("'collection'[0].'employee'.'job'", containsString("Billing"))
                .body("'collection'[0].'employee'.'salary'", numberMatches(5000.0))
                .body("'collection'[0].'employee'.'manager'.'employeeId'", numberMatches(4.0))
                .body("'collection'[0].'employee'.'manager'.'firstName'", containsString("Soumaya"))
                .body("'collection'[0].'employee'.'manager'.'lastName'", containsString("Hajjem"))
                .body("'collection'[0].'employee'.'manager'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[0].'employee'.'manager'.'phone'", containsString("22125144"))
                .body("'collection'[0].'employee'.'manager'.'hiredate'", nullValue())
                .body("'collection'[0].'employee'.'manager'.'job'", containsString("Chef service Billing"))
                .body("'collection'[0].'employee'.'manager'.'salary'", numberMatches(6000.0))
                .body("'collection'[0].'employee'.'manager'.'manager'", nullValue())
                .body("'collection'[0].'employee'.'manager'.'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[0].'employee'.'manager'.'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[0].'employee'.'manager'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[0].'employee'.'manager'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[0].'employee'.'manager'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[0].'employee'.'manager'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[0].'employee'.'manager'.'credential'.'credentialId'", numberMatches(5.0))
                .body("'collection'[0].'employee'.'manager'.'credential'.'username'", containsString("soumayahajjem"))
                .body("'collection'[0].'employee'.'manager'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[0].'employee'.'manager'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[0].'employee'.'manager'.'credential'.'role'", containsString("ROLE_MGR"))
                .body("'collection'[0].'employee'.'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[0].'employee'.'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[0].'employee'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[0].'employee'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[0].'employee'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[0].'employee'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[0].'employee'.'credential'.'credentialId'", numberMatches(3.0))
                .body("'collection'[0].'employee'.'credential'.'username'", containsString("selimhorri"))
                .body("'collection'[0].'employee'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[0].'employee'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[0].'employee'.'credential'.'role'", containsString("ROLE_EMP"))
                .body("'collection'[0].'project'.'projectId'", numberMatches(1.0))
                .body("'collection'[0].'project'.'title'", containsString("TRANSBSCS"))
                .body("'collection'[0].'project'.'startDate'", containsString("28-09-2020"))
                .body("'collection'[0].'project'.'endDate'", containsString("04-11-2020"))
                .body("'collection'[0].'project'.'status'", containsString("COMPLETED"))
                .body("'collection'[1].'employeeId'", numberMatches(1.0))
                .body("'collection'[1].'projectId'", numberMatches(1.0))
                .body("'collection'[1].'commitDate'", containsString("26-11-202013:14:22"))
                .body("'collection'[1].'commitEmpDesc'", containsString("set up some configs"))
                .body("'collection'[1].'commitMgrDesc'", containsString("you need to implement sec solution"))
                .body("'collection'[1].'employee'.'employeeId'", numberMatches(1.0))
                .body("'collection'[1].'employee'.'firstName'", containsString("Selim"))
                .body("'collection'[1].'employee'.'lastName'", containsString("Horri"))
                .body("'collection'[1].'employee'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[1].'employee'.'phone'", containsString("22125144"))
                .body("'collection'[1].'employee'.'hiredate'", containsString("15-04-2019"))
                .body("'collection'[1].'employee'.'job'", containsString("Billing"))
                .body("'collection'[1].'employee'.'salary'", numberMatches(5000.0))
                .body("'collection'[1].'employee'.'manager'.'employeeId'", numberMatches(4.0))
                .body("'collection'[1].'employee'.'manager'.'firstName'", containsString("Soumaya"))
                .body("'collection'[1].'employee'.'manager'.'lastName'", containsString("Hajjem"))
                .body("'collection'[1].'employee'.'manager'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[1].'employee'.'manager'.'phone'", containsString("22125144"))
                .body("'collection'[1].'employee'.'manager'.'hiredate'", nullValue())
                .body("'collection'[1].'employee'.'manager'.'job'", containsString("Chef service Billing"))
                .body("'collection'[1].'employee'.'manager'.'salary'", numberMatches(6000.0))
                .body("'collection'[1].'employee'.'manager'.'manager'", nullValue())
                .body("'collection'[1].'employee'.'manager'.'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[1].'employee'.'manager'.'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[1].'employee'.'manager'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[1].'employee'.'manager'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[1].'employee'.'manager'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[1].'employee'.'manager'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[1].'employee'.'manager'.'credential'.'credentialId'", numberMatches(5.0))
                .body("'collection'[1].'employee'.'manager'.'credential'.'username'", containsString("soumayahajjem"))
                .body("'collection'[1].'employee'.'manager'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[1].'employee'.'manager'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[1].'employee'.'manager'.'credential'.'role'", containsString("ROLE_MGR"))
                .body("'collection'[1].'employee'.'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[1].'employee'.'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[1].'employee'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[1].'employee'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[1].'employee'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[1].'employee'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[1].'employee'.'credential'.'credentialId'", numberMatches(3.0))
                .body("'collection'[1].'employee'.'credential'.'username'", containsString("selimhorri"))
                .body("'collection'[1].'employee'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[1].'employee'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[1].'employee'.'credential'.'role'", containsString("ROLE_EMP"))
                .body("'collection'[1].'project'.'projectId'", numberMatches(1.0))
                .body("'collection'[1].'project'.'title'", containsString("TRANSBSCS"))
                .body("'collection'[1].'project'.'startDate'", containsString("28-09-2020"))
                .body("'collection'[1].'project'.'endDate'", containsString("04-11-2020"))
                .body("'collection'[1].'project'.'status'", containsString("COMPLETED"))
                .body("'collection'[2].'employeeId'", numberMatches(1.0))
                .body("'collection'[2].'projectId'", numberMatches(1.0))
                .body("'collection'[2].'commitDate'", containsString("12-12-202016:49:42"))
                .body("'collection'[2].'commitEmpDesc'", containsString("implement customer by invoice"))
                .body("'collection'[2].'commitMgrDesc'", nullValue())
                .body("'collection'[2].'employee'.'employeeId'", numberMatches(1.0))
                .body("'collection'[2].'employee'.'firstName'", containsString("Selim"))
                .body("'collection'[2].'employee'.'lastName'", containsString("Horri"))
                .body("'collection'[2].'employee'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[2].'employee'.'phone'", containsString("22125144"))
                .body("'collection'[2].'employee'.'hiredate'", containsString("15-04-2019"))
                .body("'collection'[2].'employee'.'job'", containsString("Billing"))
                .body("'collection'[2].'employee'.'salary'", numberMatches(5000.0))
                .body("'collection'[2].'employee'.'manager'.'employeeId'", numberMatches(4.0))
                .body("'collection'[2].'employee'.'manager'.'firstName'", containsString("Soumaya"))
                .body("'collection'[2].'employee'.'manager'.'lastName'", containsString("Hajjem"))
                .body("'collection'[2].'employee'.'manager'.'email'", containsString("springabcxyzboot@gmail.com"))
                .body("'collection'[2].'employee'.'manager'.'phone'", containsString("22125144"))
                .body("'collection'[2].'employee'.'manager'.'hiredate'", nullValue())
                .body("'collection'[2].'employee'.'manager'.'job'", containsString("Chef service Billing"))
                .body("'collection'[2].'employee'.'manager'.'salary'", numberMatches(6000.0))
                .body("'collection'[2].'employee'.'manager'.'manager'", nullValue())
                .body("'collection'[2].'employee'.'manager'.'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[2].'employee'.'manager'.'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[2].'employee'.'manager'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[2].'employee'.'manager'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[2].'employee'.'manager'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[2].'employee'.'manager'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[2].'employee'.'manager'.'credential'.'credentialId'", numberMatches(5.0))
                .body("'collection'[2].'employee'.'manager'.'credential'.'username'", containsString("soumayahajjem"))
                .body("'collection'[2].'employee'.'manager'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[2].'employee'.'manager'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[2].'employee'.'manager'.'credential'.'role'", containsString("ROLE_MGR"))
                .body("'collection'[2].'employee'.'department'.'departmentId'", numberMatches(6.0))
                .body("'collection'[2].'employee'.'department'.'departmentName'", containsString("Billing"))
                .body("'collection'[2].'employee'.'department'.'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[2].'employee'.'department'.'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[2].'employee'.'department'.'location'.'postalCode'", containsString("2016"))
                .body("'collection'[2].'employee'.'department'.'location'.'city'", containsString("LAC2"))
                .body("'collection'[2].'employee'.'credential'.'credentialId'", numberMatches(3.0))
                .body("'collection'[2].'employee'.'credential'.'username'", containsString("selimhorri"))
                .body("'collection'[2].'employee'.'credential'.'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[2].'employee'.'credential'.'enabled'", equalTo(true))
                .body("'collection'[2].'employee'.'credential'.'role'", containsString("ROLE_EMP"))
                .body("'collection'[2].'project'.'projectId'", numberMatches(1.0))
                .body("'collection'[2].'project'.'title'", containsString("TRANSBSCS"))
                .body("'collection'[2].'project'.'startDate'", containsString("28-09-2020"))
                .body("'collection'[2].'project'.'endDate'", containsString("04-11-2020"))
                .body("'collection'[2].'project'.'status'", containsString("COMPLETED"))
                ; // Skipping assertions on the remaining 56 elements. This limit of 3 elements can be increased in the configurations
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-18"></a>
<details open>
<summary><b>test_18</b> &middot; F200 &middot; <code>GET:/app/api/assignments/{employeeId}/{projectId}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/assignments/{employeeId}/{projectId}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_18() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/{employeeId}/{projectId} -> Response status 400 not defined for path '/api/assignments/{employeeId}/{projectId}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "_EM_20_XYZ_")
                .get(baseUrlOfSut + "/app/api/assignments/_EM_18_XYZ_/_EM_19_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("HttpStatus must not be null"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-19"></a>
<details open>
<summary><b>test_19</b> &middot; F200 &middot; <code>POST:/app/api/projects</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/projects
    * Found 1 potential fault of type-code 200
    * Using 1 example:
    *   dd-MM-yyyy
    */
    @Test @Timeout(60)
    public void test_19() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("LOCATIONS", 142L)
                .d("ADR", "\"J8uD\"")
                .d("POSTAL_CODE", "\"PCtWRt9fTl_jGFJa\"")
                .d("CITY", "\"PYpR\"")
            .and().insertInto("LOCATIONS", 139L)
                .d("ADR", "\"IzLSuitVf8s8Fk3\"")
                .d("POSTAL_CODE", "\"zSj2\"")
                .d("CITY", "\"20c\"")
            .and().insertInto("LOCATIONS", 136L)
                .d("ADR", "\"1\"")
                .d("POSTAL_CODE", "\"qVDP2ECm3HglIUI\"")
                .d("CITY", "\"N7yqqMOTT\"")
            .and().insertInto("ASSIGNMENTS", 133L)
                .d("EMPLOYEE_ID", "12")
                .d("PROJECT_ID", "9")
                .d("COMMIT_DATE", "\"2071-10-13 09:24:55\"")
                .d("COMMIT_EMP_DESC", "\"0746OBdn1\"")
                .d("COMMIT_MGR_DESC", "NULL")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/projects -> Response status 400 not defined for path '/api/projects'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .contentType("application/json")
                .body(" { " + 
                    " \"endDate\": \"Wqv0TJI2AlNI\", " + 
                    " \"projectId\": 684, " + 
                    " \"startDate\": \"dd-MM-yyyy\", " + 
                    " \"title\": \"Rgv69OCx\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/projects")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"Wqv0TJI2AlNI\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'Wqv0TJI2AlNI' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"Wqv0TJI2AlNI\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'Wqv0TJI2AlNI' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 12] (through reference chain: com.pfa.app.model.entity.Project[\"endDate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-20"></a>
<details open>
<summary><b>test_20</b> &middot; F200 &middot; <code>POST:/app/api/projects/save</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/projects/save
    * Found 1 potential fault of type-code 200
    * Using 1 example:
    *   dd-MM-yyyy
    */
    @Test @Timeout(60)
    public void test_20() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/projects/save -> Response status 400 not defined for path '/api/projects/save'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "42")
                .contentType("application/json")
                .body(" { " + 
                    " \"endDate\": \"dd-MM-yyyy\", " + 
                    " \"projectId\": 993, " + 
                    " \"status\": \"L\", " + 
                    " \"title\": \"CAupGxCXIVblTeB\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/projects/save?EMextraParam123=42")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 12] (through reference chain: com.pfa.app.model.entity.Project[\"endDate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-21"></a>
<details open>
<summary><b>test_21</b> &middot; F200 &middot; <code>DELETE:/app/api/assignments/delete/{employeeId}/{projectId}/{commitDate}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/assignments/delete/{employeeId}/{projectId}/{commitDate}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_21() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/assignments/delete/{employeeId}/{projectId}/{commitDate} -> Response status 400 not defined for path '/api/assignments/delete/{employeeId}/{projectId}/{commitDate}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "_EM_8_XYZ_")
                .delete(baseUrlOfSut + "/app/api/assignments/delete/IdJKO1g/_EM_6_XYZ_/_EM_5_XYZ_?EMextraParam123=_EM_7_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"IdJKO1g\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-22"></a>
<details open>
<summary><b>test_22</b> &middot; F200 &middot; <code>GET:/app/api/employees/data/department/{departmentId}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/employees/data/department/{departmentId}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_22() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/data/department/{departmentId} -> Response status 400 not defined for path '/api/employees/data/department/{departmentId}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "_EM_15_XYZ_")
                .get(baseUrlOfSut + "/app/api/employees/data/department/nvUVjYS?EMextraParam123=_EM_14_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"nvUVjYS\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-23"></a>
<details open>
<summary><b>test_23</b> &middot; F200 &middot; <code>DELETE:/app/api/departments/delete/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/departments/delete/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_23() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/departments/delete/{id} -> Response status 400 not defined for path '/api/departments/delete/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "_EM_24_XYZ_")
                .delete(baseUrlOfSut + "/app/api/departments/delete/1dMK5kwtYSQKYPjC?EMextraParam123=_EM_23_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"1dMK5kwtYSQKYPjC\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-24"></a>
<details open>
<summary><b>test_24</b> &middot; F200 &middot; <code>DELETE:/app/api/employees/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/employees/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_24() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/employees/{id} -> Response status 400 not defined for path '/api/employees/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "_EM_43_XYZ_")
                .delete(baseUrlOfSut + "/app/api/employees/OaF6He")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"OaF6He\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-25"></a>
<details open>
<summary><b>test_25</b> &middot; F200 &middot; <code>DELETE:/app/api/locations/delete/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/locations/delete/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_25() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/locations/delete/{id} -> Response status 400 not defined for path '/api/locations/delete/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "42")
                .delete(baseUrlOfSut + "/app/api/locations/delete/FVVwKoYGzNdBUSRN?EMextraParam123=_EM_26_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"FVVwKoYGzNdBUSRN\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-26"></a>
<details open>
<summary><b>test_26</b> &middot; F200 &middot; <code>DELETE:/app/api/projects/delete/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/projects/delete/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_26() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/projects/delete/{id} -> Response status 400 not defined for path '/api/projects/delete/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .delete(baseUrlOfSut + "/app/api/projects/delete/ZqGYwxwopuxsihuC")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"ZqGYwxwopuxsihuC\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-27"></a>
<details open>
<summary><b>test_27</b> &middot; F200 &middot; <code>GET:/app/api/departments/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/departments/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_27() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/departments/{id} -> Response status 400 not defined for path '/api/departments/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/departments/s6")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"s6\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-28"></a>
<details open>
<summary><b>test_28</b> &middot; F200 &middot; <code>PUT:/app/api/projects</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/projects
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_28() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("PROJECTS", 143L)
                .d("TITLE", "\"b\"")
                .d("STATUS", "\"G4cNxWPAvx\"")
            .and().insertInto("LOCATIONS", 142L)
                .d("ADR", "\"J8uD\"")
                .d("POSTAL_CODE", "\"PCtWRt9fTl_jGFJa\"")
                .d("CITY", "\"PYpR\"")
            .and().insertInto("DEPARTMENTS", 141L)
                .d("DEPARTMENT_NAME", "\"_ggIRn8pCZdpTh7\"")
            .and().insertInto("EMPLOYEES", 140L)
                .d("FIRST_NAME", "\"4SIYyQN\"")
                .d("LAST_NAME", "\"Jf\"")
                .d("EMAIL", "\"UKs@sd.XAe\"")
                .d("PHONE", "\"p\"")
                .d("JOB", "\"r\"")
                .d("SALARY", "0.6060128345707113")
            .and().insertInto("LOCATIONS", 139L)
                .d("ADR", "\"IzLSuitVf8s8Fk3\"")
                .d("POSTAL_CODE", "\"zSj2\"")
                .d("CITY", "\"20c\"")
            .and().insertInto("DEPARTMENTS", 138L)
                .d("DEPARTMENT_NAME", "\"PKyExGenGGWaJ\"")
            .and().insertInto("EMPLOYEES", 137L)
                .d("FIRST_NAME", "\"x3b6rVD7esITb\"")
                .d("LAST_NAME", "\"gIf\"")
                .d("EMAIL", "\"Fv@h.DHHg\"")
                .d("PHONE", "\"GjlJrEDdeg\"")
                .d("JOB", "\"lcoeYTmySWh\"")
                .d("SALARY", "0.23306002734306475")
            .and().insertInto("LOCATIONS", 136L)
                .d("ADR", "\"1\"")
                .d("POSTAL_CODE", "\"qVDP2ECm3HglIUI\"")
                .d("CITY", "\"N7yqqMOTT\"")
            .and().insertInto("DEPARTMENTS", 135L)
                .d("DEPARTMENT_NAME", "\"0shXKRn\"")
            .and().insertInto("EMPLOYEES", 134L)
                .d("FIRST_NAME", "\"q8FFL8Blw5U\"")
                .d("LAST_NAME", "\"a\"")
                .d("EMAIL", "\"HTb@q.ZR\"")
                .d("PHONE", "\"Z9oGzZ\"")
                .d("JOB", "\"9j\"")
                .d("SALARY", "0.6189236806865404")
            .and().insertInto("ASSIGNMENTS", 133L)
                .d("EMPLOYEE_ID", "12")
                .d("PROJECT_ID", "9")
                .d("COMMIT_DATE", "\"2071-10-13 09:24:55\"")
                .d("COMMIT_EMP_DESC", "\"0746OBdn1\"")
                .d("COMMIT_MGR_DESC", "NULL")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/projects -> Response status 400 not defined for path '/api/projects'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .contentType("application/json")
                .body(" { " + 
                    " \"endDate\": \"mRxcIhXyWj\", " + 
                    " \"projectId\": 397, " + 
                    " \"startDate\": \"\", " + 
                    " \"status\": \"QqBr1o8CH4jL\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/projects?password=6vsVo9Vy")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"mRxcIhXyWj\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'mRxcIhXyWj' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"mRxcIhXyWj\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'mRxcIhXyWj' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 12] (through reference chain: com.pfa.app.model.entity.Project[\"endDate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-29"></a>
<details open>
<summary><b>test_29</b> &middot; F200 &middot; <code>PUT:/app/api/projects</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/projects
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_29() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("PROJECTS", 143L)
                .d("TITLE", "\"b\"")
                .d("STATUS", "\"G4cNwWPAvx\"")
            .and().insertInto("LOCATIONS", 142L)
                .d("ADR", "\"J8uD\"")
                .d("POSTAL_CODE", "\"PCtWRt9fTl_jGFJa\"")
                .d("CITY", "\"PYpR\"")
            .and().insertInto("DEPARTMENTS", 141L)
                .d("DEPARTMENT_NAME", "\"_ggIRn8pCZdpTh7\"")
            .and().insertInto("EMPLOYEES", 140L)
                .d("FIRST_NAME", "\"4SIYyQN\"")
                .d("LAST_NAME", "\"Jf\"")
                .d("EMAIL", "\"UKs@sd.XAe\"")
                .d("PHONE", "\"p\"")
                .d("JOB", "\"r\"")
                .d("SALARY", "0.6060128345707113")
            .and().insertInto("LOCATIONS", 139L)
                .d("ADR", "\"IzLSuitVf8s8Fk3\"")
                .d("POSTAL_CODE", "\"zSj2\"")
                .d("CITY", "\"20c\"")
            .and().insertInto("DEPARTMENTS", 138L)
                .d("DEPARTMENT_NAME", "\"PKyExGenGGWaJ\"")
            .and().insertInto("EMPLOYEES", 137L)
                .d("FIRST_NAME", "\"x3b6rVD7esITb\"")
                .d("LAST_NAME", "\"gIf\"")
                .d("EMAIL", "\"Fv@h.DHHg\"")
                .d("PHONE", "\"GjlJrEDdeg\"")
                .d("JOB", "\"lcoeYTmySWh\"")
                .d("SALARY", "0.23306002734306475")
            .and().insertInto("LOCATIONS", 136L)
                .d("ADR", "\"1\"")
                .d("POSTAL_CODE", "\"qVDP2ECm3HglIUI\"")
                .d("CITY", "\"N7yqqMOTT\"")
            .and().insertInto("DEPARTMENTS", 135L)
                .d("DEPARTMENT_NAME", "\"0shXKRn\"")
            .and().insertInto("EMPLOYEES", 134L)
                .d("FIRST_NAME", "\"q8FFL8Blw5U\"")
                .d("LAST_NAME", "\"a\"")
                .d("EMAIL", "\"HTb@q.ZR\"")
                .d("PHONE", "\"Z9oGzZ\"")
                .d("JOB", "\"9j\"")
                .d("SALARY", "0.6189236806865404")
            .and().insertInto("ASSIGNMENTS", 133L)
                .d("EMPLOYEE_ID", "12")
                .d("PROJECT_ID", "9")
                .d("COMMIT_DATE", "\"2071-10-13 09:24:55\"")
                .d("COMMIT_EMP_DESC", "\"0746OBdn1\"")
                .d("COMMIT_MGR_DESC", "NULL")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/projects -> Response status 400 not defined for path '/api/projects'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .contentType("application/json")
                .body(" { " + 
                    " \"endDate\": \"mRxcIhXyHWj\", " + 
                    " \"projectId\": 397, " + 
                    " \"startDate\": \"W\", " + 
                    " \"status\": \"QqBr1o8CH4jL\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/projects?" + 
                    "password=6vsVo9Vy&" + 
                    "username=QP2C")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"mRxcIhXyHWj\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'mRxcIhXyHWj' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"mRxcIhXyHWj\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'mRxcIhXyHWj' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 12] (through reference chain: com.pfa.app.model.entity.Project[\"endDate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-30"></a>
<details open>
<summary><b>test_30</b> &middot; F200 &middot; <code>GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_30() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId} -> Response status 400 not defined for path '/api/assignments/data/project-commit/{employeeId}/{projectId}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/assignments/data/project-commit/_EM_3_XYZ_/K2GtpPR?EMextraParam123=42")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"_EM_3_XYZ_\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-31"></a>
<details open>
<summary><b>test_31</b> &middot; F200 &middot; <code>GET:/app/api/assignments/{employeeId}/{projectId}/{commitDate}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/assignments/{employeeId}/{projectId}/{commitDate}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_31() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/{employeeId}/{projectId}/{commitDate} -> Response status 400 not defined for path '/api/assignments/{employeeId}/{projectId}/{commitDate}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/assignments/_EM_9_XYZ_/_EM_10_XYZ_/4TJ8UbWe?EMextraParam123=_EM_11_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"_EM_9_XYZ_\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-32"></a>
<details open>
<summary><b>test_32</b> &middot; F200 &middot; <code>GET:/app/api/employees/data/manager-project-data/{employeeId}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/employees/data/manager-project-data/{employeeId}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_32() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/data/manager-project-data/{employeeId} -> Response status 400 not defined for path '/api/employees/data/manager-project-data/{employeeId}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/employees/data/manager-project-data/_EM_16_XYZ_?EMextraParam123=_EM_17_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"_EM_16_XYZ_\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-33"></a>
<details open>
<summary><b>test_33</b> &middot; F200 &middot; <code>DELETE:/app/api/credentials/delete/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/credentials/delete/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_33() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/credentials/delete/{id} -> Response status 400 not defined for path '/api/credentials/delete/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "_EM_22_XYZ_")
                .delete(baseUrlOfSut + "/app/api/credentials/delete/_EM_21_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"_EM_21_XYZ_\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-34"></a>
<details open>
<summary><b>test_34</b> &middot; F200 &middot; <code>GET:/app/api/credentials/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/credentials/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_34() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/credentials/{id} -> Response status 400 not defined for path '/api/credentials/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "_EM_30_XYZ_")
                .get(baseUrlOfSut + "/app/api/credentials/_EM_29_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"_EM_29_XYZ_\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-35"></a>
<details open>
<summary><b>test_35</b> &middot; F200 &middot; <code>GET:/app/api/employees/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/employees/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_35() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/{id} -> Response status 400 not defined for path '/api/employees/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "_EM_41_XYZ_")
                .get(baseUrlOfSut + "/app/api/employees/_EM_39_XYZ_?EMextraParam123=_EM_40_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"_EM_39_XYZ_\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-36"></a>
<details open>
<summary><b>test_36</b> &middot; F200 &middot; <code>GET:/app/api/projects/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/projects/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_36() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/projects/{id} -> Response status 400 not defined for path '/api/projects/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/projects/_EM_47_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"_EM_47_XYZ_\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-37"></a>
<details open>
<summary><b>test_37</b> &middot; F200 &middot; <code>DELETE:/app/api/projects/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/projects/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_37() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/projects/{id} -> Response status 400 not defined for path '/api/projects/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .delete(baseUrlOfSut + "/app/api/projects/_EM_49_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"_EM_49_XYZ_\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-38"></a>
<details open>
<summary><b>test_38</b> &middot; F200 &middot; <code>DELETE:/app/api/credentials/username/{username}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/credentials/username/{username}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_38() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/credentials/username/{username} -> Response status 400 not defined for path '/api/credentials/username/{username}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .delete(baseUrlOfSut + "/app/api/credentials/username/_EM_28_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("###### NO Credential object FOUND with username: _EM_28_XYZ_ ! ######"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-39"></a>
<details open>
<summary><b>test_39</b> &middot; F200 &middot; <code>GET:/app/api/employees/username/{username}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/employees/username/{username}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_39() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/username/{username} -> Response status 400 not defined for path '/api/employees/username/{username}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "42")
                .get(baseUrlOfSut + "/app/api/employees/username/_EM_36_XYZ_?EMextraParam123=_EM_37_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("###### NO Credential object FOUND with username: _EM_36_XYZ_ ! ######"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-40"></a>
<details open>
<summary><b>test_40</b> &middot; F200 &middot; <code>GET:/app/api/credentials/username/{username}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/credentials/username/{username}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_40() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("PROJECTS", 143L)
                .d("TITLE", "\"b\"")
                .d("STATUS", "\"G4cNxWPAvx\"")
            .and().insertInto("LOCATIONS", 142L)
                .d("ADR", "\"J8uD\"")
                .d("POSTAL_CODE", "\"PCtWRt9fTl_jGFJa\"")
                .d("CITY", "\"PYpR\"")
            .and().insertInto("DEPARTMENTS", 141L)
                .d("DEPARTMENT_NAME", "\"_ggIRn8pCZdpTh7\"")
            .and().insertInto("EMPLOYEES", 140L)
                .d("FIRST_NAME", "\"4SIYyQN\"")
                .d("LAST_NAME", "\"Jf\"")
                .d("EMAIL", "\"UKs@sd.XAe\"")
                .d("PHONE", "\"p\"")
                .d("JOB", "\"r\"")
                .d("SALARY", "0.6060128345707113")
            .and().insertInto("LOCATIONS", 139L)
                .d("ADR", "\"IzLSuitVf8s8Fk3\"")
                .d("POSTAL_CODE", "\"zSj2\"")
                .d("CITY", "\"20c\"")
            .and().insertInto("DEPARTMENTS", 138L)
                .d("DEPARTMENT_NAME", "\"PKyExGenGGWaJ\"")
            .and().insertInto("EMPLOYEES", 137L)
                .d("FIRST_NAME", "\"x3b6rVD7esITb\"")
                .d("LAST_NAME", "\"gIf\"")
                .d("EMAIL", "\"Fv@h.DHHg\"")
                .d("PHONE", "\"GjlJrEDdeg\"")
                .d("JOB", "\"lcoeYTmySWh\"")
                .d("SALARY", "0.23306002734306475")
            .and().insertInto("LOCATIONS", 136L)
                .d("ADR", "\"1\"")
                .d("POSTAL_CODE", "\"qVDP2ECm3HglIUI\"")
                .d("CITY", "\"N7yqqMOTT\"")
            .and().insertInto("DEPARTMENTS", 135L)
                .d("DEPARTMENT_NAME", "\"0shXKRn\"")
            .and().insertInto("EMPLOYEES", 134L)
                .d("FIRST_NAME", "\"q8FFL8Blw5U\"")
                .d("LAST_NAME", "\"a\"")
                .d("EMAIL", "\"HTb@q.ZR\"")
                .d("PHONE", "\"Z9oGzZ\"")
                .d("JOB", "\"9j\"")
                .d("SALARY", "0.6189236806865404")
            .and().insertInto("ASSIGNMENTS", 133L)
                .d("EMPLOYEE_ID", "12")
                .d("PROJECT_ID", "9")
                .d("COMMIT_DATE", "\"2071-10-13 09:24:55\"")
                .d("COMMIT_EMP_DESC", "\"0746OBdn1\"")
                .d("COMMIT_MGR_DESC", "NULL")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/credentials/username/{username} -> Response status 400 not defined for path '/api/credentials/username/{username}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/credentials/username/ceJohDIBfm")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("###### NO Credential object FOUND with username: ceJohDIBfm ! ######"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-41"></a>
<details open>
<summary><b>test_41</b> &middot; F200 &middot; <code>PUT:/app/api/assignments</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/assignments
    * Found 1 potential fault of type-code 200
    * Using 1 example:
    *   dd-MM-yyyyHH:mm:ss
    */
    @Test @Timeout(60)
    public void test_41() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/assignments -> Response status 400 not defined for path '/api/assignments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "42")
                .contentType("application/json")
                .body(" { " + 
                    " \"commitDate\": \"dd-MM-yyyyHH:mm:ss\", " + 
                    " \"commitMgrDesc\": \"p508Asdp_\", " + 
                    " \"employee\": { " + 
                    " \"credential\": { " + 
                    " \"password\": \"_EM_250_XYZ_\", " + 
                    " \"username\": \"_EM_252_XYZ_\" " + 
                    " }, " + 
                    " \"department\": { " + 
                    " \"location\": { " + 
                    " \"locationId\": 724 " + 
                    " } " + 
                    " }, " + 
                    " \"email\": \"rn35t30WfU\", " + 
                    " \"job\": \"_EM_255_XYZ_\", " + 
                    " \"lastName\": \"Chaouachi\" " + 
                    " } " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/assignments")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDateTime` from String \"dd-MM-yyyyHH:mm:ss\": Failed to deserialize java.time.LocalDateTime: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyyHH:mm:ss' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDateTime` from String \"dd-MM-yyyyHH:mm:ss\": Failed to deserialize java.time.LocalDateTime: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyyHH:mm:ss' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 15] (through reference chain: com.pfa.app.model.entity.Assignment[\"commitDate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-42"></a>
<details open>
<summary><b>test_42</b> &middot; F200 &middot; <code>GET:/app/api/credentials/username/{username}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/credentials/username/{username}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_42() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("PROJECTS", 143L)
                .d("TITLE", "\"b\"")
                .d("STATUS", "\"G4cNxWPAvx\"")
            .and().insertInto("LOCATIONS", 142L)
                .d("ADR", "\"J8uD\"")
                .d("POSTAL_CODE", "\"PCtWRt9fTl_jGFJa\"")
                .d("CITY", "\"PYpR\"")
            .and().insertInto("DEPARTMENTS", 141L)
                .d("DEPARTMENT_NAME", "\"_ggIRn8pCZdpTh7\"")
            .and().insertInto("EMPLOYEES", 140L)
                .d("FIRST_NAME", "\"4SIYyQN\"")
                .d("LAST_NAME", "\"Jf\"")
                .d("EMAIL", "\"UKs@sd.XAe\"")
                .d("PHONE", "\"p\"")
                .d("JOB", "\"r\"")
                .d("SALARY", "0.6060128345707113")
            .and().insertInto("LOCATIONS", 139L)
                .d("ADR", "\"IzLSuitVf8s8Fk3\"")
                .d("POSTAL_CODE", "\"zSj2\"")
                .d("CITY", "\"20c\"")
            .and().insertInto("DEPARTMENTS", 138L)
                .d("DEPARTMENT_NAME", "\"PKyExGenGGWaJ\"")
            .and().insertInto("EMPLOYEES", 137L)
                .d("FIRST_NAME", "\"x3b6rVD7esITb\"")
                .d("LAST_NAME", "\"gIf\"")
                .d("EMAIL", "\"Fv@h.DHHg\"")
                .d("PHONE", "\"GjlJrEDdeg\"")
                .d("JOB", "\"lcoeYTmySWh\"")
                .d("SALARY", "0.23306002734306475")
            .and().insertInto("LOCATIONS", 136L)
                .d("ADR", "\"1\"")
                .d("POSTAL_CODE", "\"qVDP2ECm3HglIUI\"")
                .d("CITY", "\"N7yqqMOTT\"")
            .and().insertInto("DEPARTMENTS", 135L)
                .d("DEPARTMENT_NAME", "\"0shXKRn\"")
            .and().insertInto("EMPLOYEES", 134L)
                .d("FIRST_NAME", "\"q8FFL8Blw5U\"")
                .d("LAST_NAME", "\"a\"")
                .d("EMAIL", "\"HTb@q.ZR\"")
                .d("PHONE", "\"Z9oGzZ\"")
                .d("JOB", "\"9j\"")
                .d("SALARY", "0.6189236806865404")
            .and().insertInto("ASSIGNMENTS", 133L)
                .d("EMPLOYEE_ID", "12")
                .d("PROJECT_ID", "9")
                .d("COMMIT_DATE", "\"2071-10-13 09:24:55\"")
                .d("COMMIT_EMP_DESC", "\"0746OBdn1\"")
                .d("COMMIT_MGR_DESC", "NULL")
            .and().insertInto("LOCATIONS", 153L)
                .d("ADR", "\"qrm4ziL6X\"")
                .d("POSTAL_CODE", "\"jtsOAJjqyr\"")
                .d("CITY", "\"3YKvJ0\"")
            .and().insertInto("DEPARTMENTS", 152L)
                .d("DEPARTMENT_NAME", "\"2eJrsTfp\"")
            .and().insertInto("EMPLOYEES", 151L)
                .d("FIRST_NAME", "\"O6klnDzgzZ2FzX\"")
                .d("LAST_NAME", "\"Cx9FrV5K2SGY\"")
                .d("EMAIL", "\"qO@z.synX\"")
                .d("PHONE", "\"YF4cwKXt\"")
                .d("JOB", "\"JS7OrMwkio7\"")
                .d("SALARY", "0.3099283709653814")
            .and().insertInto("EMPLOYEES", 148L)
                .d("FIRST_NAME", "\"yM14\"")
                .d("LAST_NAME", "\"hhXjMynnQ\"")
                .d("EMAIL", "\"nphp@w.MY\"")
                .d("PHONE", "\"\"")
                .d("JOB", "\"4DDOXSnV6B\"")
                .d("SALARY", "0.2269540442242557")
            .and().insertInto("USER_CREDENTIALS", 144L)
                .d("USERNAME", "NULL")
                .d("PASSWORD", "\"vMuoNGbiuPekaVLt\"")
                .d("ENABLED", "true")
                .d("ROLE", "\"KU\"")
                .d("EMPLOYEE_ID", "NULL")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/credentials/username/{username} -> Response status 400 not defined for path '/api/credentials/username/{username}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/credentials/username/ceJohDIBfm?" + 
                    "password=aOzT_nFXeb67NIC3&" + 
                    "username=BWFEdeljOm")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("###### NO Credential object FOUND with username: ceJohDIBfm ! ######"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-43"></a>
<details open>
<summary><b>test_43</b> &middot; F200 &middot; <code>POST:/app/api/locations/save</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/locations/save
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_43() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/locations/save -> Response status 400 not defined for path '/api/locations/save'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "42")
                .contentType("application/json")
                .body(" { " + 
                    " \"postalCode\": \"_EM_81_XYZ_\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/locations/save?EMextraParam123=42")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Validation failed for classes [com.pfa.app.model.entity.Location] during persist time for groups [javax.validation.groups.Default, ]\nList of constraint violations:[\n\tConstraintViolationImpl{interpolatedMessage='*Must Not blank**', propertyPath=city, rootBeanClass=class com.pfa.app.model.entity.Location, messageTemplate='*Must Not blank**'}\n\tConstraintViolationImpl{interpolatedMessage='*Must Not blank**', propertyPath=adr, rootBeanClass=class com.pfa.app.model.entity.Location, messageTemplate='*Must Not blank**'}\n]"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-44"></a>
<details open>
<summary><b>test_44</b> &middot; F200 &middot; <code>PUT:/app/api/locations/update</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/locations/update
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_44() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/locations/update -> Response status 400 not defined for path '/api/locations/update'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .contentType("application/json")
                .body(" { " + 
                    " \"adr\": \"RUE DE BLA BLA\", " + 
                    " \"locationId\": 546 " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/locations/update")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Validation failed for classes [com.pfa.app.model.entity.Location] during persist time for groups [javax.validation.groups.Default, ]\nList of constraint violations:[\n\tConstraintViolationImpl{interpolatedMessage='*Must Not blank**', propertyPath=postalCode, rootBeanClass=class com.pfa.app.model.entity.Location, messageTemplate='*Must Not blank**'}\n\tConstraintViolationImpl{interpolatedMessage='*Must Not blank**', propertyPath=city, rootBeanClass=class com.pfa.app.model.entity.Location, messageTemplate='*Must Not blank**'}\n]"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-45"></a>
<details open>
<summary><b>test_45</b> &middot; F200 &middot; <code>PUT:/app/api/departments</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/departments
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_45() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("PROJECTS", 143L)
                .d("TITLE", "\"b\"")
                .d("STATUS", "\"G4cNxWPAvx\"")
            .and().insertInto("LOCATIONS", 142L)
                .d("ADR", "\"J8uD\"")
                .d("POSTAL_CODE", "\"PCtWRt9fTl_jGFJa\"")
                .d("CITY", "\"PYpR\"")
            .and().insertInto("DEPARTMENTS", 141L)
                .d("DEPARTMENT_NAME", "\"_ggIRn8pCZdpTh7\"")
            .and().insertInto("EMPLOYEES", 140L)
                .d("FIRST_NAME", "\"4SIYyQN\"")
                .d("LAST_NAME", "\"Jf\"")
                .d("EMAIL", "\"UKs@sd.XAe\"")
                .d("PHONE", "\"p\"")
                .d("JOB", "\"r\"")
                .d("SALARY", "0.6060128345707113")
            .and().insertInto("LOCATIONS", 139L)
                .d("ADR", "\"IzLSuitVf8s8Fk3\"")
                .d("POSTAL_CODE", "\"zSj2\"")
                .d("CITY", "\"20c\"")
            .and().insertInto("DEPARTMENTS", 138L)
                .d("DEPARTMENT_NAME", "\"PKyExGenGGWaJ\"")
            .and().insertInto("EMPLOYEES", 137L)
                .d("FIRST_NAME", "\"x3b6rVD7esITb\"")
                .d("LAST_NAME", "\"gIf\"")
                .d("EMAIL", "\"Fv@h.DHHg\"")
                .d("PHONE", "\"GjlJrEDdeg\"")
                .d("JOB", "\"lcoeYTmySWh\"")
                .d("SALARY", "0.23306002734306475")
            .and().insertInto("LOCATIONS", 136L)
                .d("ADR", "\"1\"")
                .d("POSTAL_CODE", "\"qVDP2ECm3HglIUI\"")
                .d("CITY", "\"N7yqqMOTT\"")
            .and().insertInto("DEPARTMENTS", 135L)
                .d("DEPARTMENT_NAME", "\"0shXKRn\"")
            .and().insertInto("EMPLOYEES", 134L)
                .d("FIRST_NAME", "\"q8FFL8Blw5U\"")
                .d("LAST_NAME", "\"a\"")
                .d("EMAIL", "\"HTb@q.ZR\"")
                .d("PHONE", "\"Z9oGzZ\"")
                .d("JOB", "\"9j\"")
                .d("SALARY", "0.6189236806865404")
            .and().insertInto("ASSIGNMENTS", 133L)
                .d("EMPLOYEE_ID", "12")
                .d("PROJECT_ID", "9")
                .d("COMMIT_DATE", "\"2071-10-13 09:24:55\"")
                .d("COMMIT_EMP_DESC", "\"0746OBdn1\"")
                .d("COMMIT_MGR_DESC", "NULL")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/departments -> Response status 400 not defined for path '/api/departments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .contentType("application/json")
                .body(" { " + 
                    " \"departmentId\": 366, " + 
                    " \"departmentName\": \"tt5LjlA2yeX\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/departments")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Validation failed for classes [com.pfa.app.model.entity.Department] during persist time for groups [javax.validation.groups.Default, ]\nList of constraint violations:[\n\tConstraintViolationImpl{interpolatedMessage='*Must not NULL**', propertyPath=location, rootBeanClass=class com.pfa.app.model.entity.Department, messageTemplate='*Must not NULL**'}\n]"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-46"></a>
<details open>
<summary><b>test_46</b> &middot; F200 &middot; <code>PUT:/app/api/departments</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/departments
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_46() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("PROJECTS", 143L)
                .d("TITLE", "\"b\"")
                .d("STATUS", "\"G4cNxWPAvx\"")
            .and().insertInto("LOCATIONS", 142L)
                .d("ADR", "\"J8uD\"")
                .d("POSTAL_CODE", "\"PCtWRt9fTl_jGFJa\"")
                .d("CITY", "\"PYpR\"")
            .and().insertInto("DEPARTMENTS", 141L)
                .d("DEPARTMENT_NAME", "\"_ggIRn8pCZdpTh7\"")
            .and().insertInto("EMPLOYEES", 140L)
                .d("FIRST_NAME", "\"4SIYyQN\"")
                .d("LAST_NAME", "\"Jf\"")
                .d("EMAIL", "\"UKs@sd.XAe\"")
                .d("PHONE", "\"p\"")
                .d("JOB", "\"r\"")
                .d("SALARY", "0.6060128345707113")
            .and().insertInto("LOCATIONS", 139L)
                .d("ADR", "\"IzLSuitVf8s8Fk3\"")
                .d("POSTAL_CODE", "\"zSj2\"")
                .d("CITY", "\"20c\"")
            .and().insertInto("DEPARTMENTS", 138L)
                .d("DEPARTMENT_NAME", "\"PKyExGenGGWaJ\"")
            .and().insertInto("EMPLOYEES", 137L)
                .d("FIRST_NAME", "\"x3b6rVD7esITb\"")
                .d("LAST_NAME", "\"gIf\"")
                .d("EMAIL", "\"Fv@h.DHHg\"")
                .d("PHONE", "\"GjlJrEDdcg\"")
                .d("JOB", "\"lcoeYTmySWh\"")
                .d("SALARY", "0.23306002734306475")
            .and().insertInto("LOCATIONS", 136L)
                .d("ADR", "\"1\"")
                .d("POSTAL_CODE", "\"qVDP2ECm3HglIUI\"")
                .d("CITY", "\"N7yqqMOTT\"")
            .and().insertInto("DEPARTMENTS", 135L)
                .d("DEPARTMENT_NAME", "\"0shXKRn\"")
            .and().insertInto("EMPLOYEES", 134L)
                .d("FIRST_NAME", "\"q8FFL8Blw5U\"")
                .d("LAST_NAME", "\"a\"")
                .d("EMAIL", "\"HTb@q.ZR\"")
                .d("PHONE", "\"Z9oGzZ\"")
                .d("JOB", "\"9j\"")
                .d("SALARY", "0.6189236806865404")
            .and().insertInto("ASSIGNMENTS", 133L)
                .d("EMPLOYEE_ID", "12")
                .d("PROJECT_ID", "9")
                .d("COMMIT_DATE", "\"2071-10-13 09:24:55\"")
                .d("COMMIT_EMP_DESC", "\"0746OBdn1\"")
                .d("COMMIT_MGR_DESC", "NULL")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/departments -> Response status 400 not defined for path '/api/departments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .contentType("application/json")
                .body(" { " + 
                    " \"departmentId\": 366, " + 
                    " \"departmentName\": \"tt5LjlA2yeX\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/departments?" + 
                    "password=6VMIUt&" + 
                    "username=Hu")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Validation failed for classes [com.pfa.app.model.entity.Department] during persist time for groups [javax.validation.groups.Default, ]\nList of constraint violations:[\n\tConstraintViolationImpl{interpolatedMessage='*Must not NULL**', propertyPath=location, rootBeanClass=class com.pfa.app.model.entity.Department, messageTemplate='*Must not NULL**'}\n]"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-47"></a>
<details open>
<summary><b>test_47</b> &middot; F200 &middot; <code>POST:/app/api/authenticate</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/authenticate
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_47() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/authenticate -> Response status 400 not defined for path '/api/authenticate'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "42")
                .contentType("application/json")
                .body(" { " + 
                    " \"password\": \"_EM_93_XYZ_\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/authenticate")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Bad credentials"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-48"></a>
<details open>
<summary><b>test_48</b> &middot; F200 &middot; <code>PUT:/app/api/departments</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/departments
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_48() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/departments -> Response status 400 not defined for path '/api/departments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "_EM_126_XYZ_")
                .contentType("application/json")
                .body(" { " + 
                    " \"departmentId\": 435, " + 
                    " \"location\": { " + 
                    " \"adr\": \"S\", " + 
                    " \"city\": \"_EM_123_XYZ_\", " + 
                    " \"locationId\": 1 " + 
                    " } " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/departments?EMextraParam123=_EM_125_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Validation failed for classes [com.pfa.app.model.entity.Department] during persist time for groups [javax.validation.groups.Default, ]\nList of constraint violations:[\n\tConstraintViolationImpl{interpolatedMessage='*Must not blank**', propertyPath=departmentName, rootBeanClass=class com.pfa.app.model.entity.Department, messageTemplate='*Must not blank**'}\n]"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-49"></a>
<details open>
<summary><b>test_49</b> &middot; F200 &middot; <code>PUT:/app/api/employees</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/employees
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_49() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/employees -> Response status 400 not defined for path '/api/employees'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "42")
                .contentType("application/json")
                .body(" { " + 
                    " \"department\": { " + 
                    " \"departmentId\": 765, " + 
                    " \"departmentName\": \"_EM_128_XYZ_\" " + 
                    " }, " + 
                    " \"email\": \"_EM_129_XYZ_\", " + 
                    " \"employeeId\": 425, " + 
                    " \"lastName\": \"_EM_132_XYZ_\", " + 
                    " \"salary\": 0.00593367434706038 " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/employees?EMextraParam123=_EM_134_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", nullValue())
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-50"></a>
<details open>
<summary><b>test_50</b> &middot; F200 &middot; <code>PUT:/app/api/employees/update</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/employees/update
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_50() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/employees/update -> Response status 400 not defined for path '/api/employees/update'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "_EM_159_XYZ_")
                .contentType("application/json")
                .body(" { " + 
                    " \"credential\": { " + 
                    " \"credentialId\": 138, " + 
                    " \"enabled\": false, " + 
                    " \"password\": \"dFEFA\", " + 
                    " \"role\": \"_EM_154_XYZ_\", " + 
                    " \"username\": \"maryemtlemseni\" " + 
                    " }, " + 
                    " \"department\": { " + 
                    " \"departmentName\": \"0y\", " + 
                    " \"location\": { " + 
                    " \"locationId\": 480, " + 
                    " \"postalCode\": \"oc55Ajqa_hx083_\" " + 
                    " } " + 
                    " }, " + 
                    " \"hiredate\": \"AxwB\", " + 
                    " \"salary\": 0.4401792996387375 " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/employees/update")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"AxwB\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'AxwB' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"AxwB\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'AxwB' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 238] (through reference chain: com.pfa.app.model.entity.Employee[\"hiredate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-51"></a>
<details open>
<summary><b>test_51</b> &middot; F200 &middot; <code>POST:/app/api/credentials</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/credentials
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_51() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/credentials -> Response status 400 not defined for path '/api/credentials'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .contentType("application/json")
                .body(" { " + 
                    " \"credentialId\": 3, " + 
                    " \"role\": \"pEgKhuzkX\", " + 
                    " \"username\": \"_EM_407_XYZ_\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/credentials")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("could not execute statement; SQL [n/a]; constraint [null]; nested exception is org.hibernate.exception.ConstraintViolationException: could not execute statement"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-52"></a>
<details open>
<summary><b>test_52</b> &middot; F200 &middot; <code>POST:/app/api/employees/save</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/employees/save
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_52() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("PROJECTS", 143L)
                .d("TITLE", "\"b\"")
                .d("STATUS", "\"G4cNxWPAvx\"")
            .and().insertInto("LOCATIONS", 142L)
                .d("ADR", "\"J8uD\"")
                .d("POSTAL_CODE", "\"PCtWRt9fTl_jGFJa\"")
                .d("CITY", "\"PYpR\"")
            .and().insertInto("DEPARTMENTS", 141L)
                .d("DEPARTMENT_NAME", "\"_ggIRn8pCZdpTh7\"")
            .and().insertInto("EMPLOYEES", 140L)
                .d("FIRST_NAME", "\"4SIYyQN\"")
                .d("LAST_NAME", "\"Jf\"")
                .d("EMAIL", "\"UKs@sd.XAe\"")
                .d("PHONE", "\"p\"")
                .d("JOB", "\"r\"")
                .d("SALARY", "0.6060128345707113")
            .and().insertInto("LOCATIONS", 139L)
                .d("ADR", "\"IzLSuitVf8s8Fk3\"")
                .d("POSTAL_CODE", "\"zSj2\"")
                .d("CITY", "\"20c\"")
            .and().insertInto("DEPARTMENTS", 138L)
                .d("DEPARTMENT_NAME", "\"PKyExGenGGWaJ\"")
            .and().insertInto("EMPLOYEES", 137L)
                .d("FIRST_NAME", "\"x3b6rVD7esITb\"")
                .d("LAST_NAME", "\"gIf\"")
                .d("EMAIL", "\"Fv@h.DHHg\"")
                .d("PHONE", "\"GjlJrEDdeg\"")
                .d("JOB", "\"lcoeYTmySWh\"")
                .d("SALARY", "0.23306002734306475")
            .and().insertInto("LOCATIONS", 136L)
                .d("ADR", "\"1\"")
                .d("POSTAL_CODE", "\"qVDP2ECm3HglIUI\"")
                .d("CITY", "\"N7yqqMOTT\"")
            .and().insertInto("DEPARTMENTS", 135L)
                .d("DEPARTMENT_NAME", "\"0shXKRn\"")
            .and().insertInto("EMPLOYEES", 134L)
                .d("FIRST_NAME", "\"q8FFL8Blw5U\"")
                .d("LAST_NAME", "\"a\"")
                .d("EMAIL", "\"HTb@q.ZR\"")
                .d("PHONE", "\"Z9oGzZ\"")
                .d("JOB", "\"9j\"")
                .d("SALARY", "0.6189236806865404")
            .and().insertInto("ASSIGNMENTS", 133L)
                .d("EMPLOYEE_ID", "12")
                .d("PROJECT_ID", "9")
                .d("COMMIT_DATE", "\"2071-10-13 09:24:55\"")
                .d("COMMIT_EMP_DESC", "\"0746OBdn1\"")
                .d("COMMIT_MGR_DESC", "NULL")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/employees/save -> Response status 400 not defined for path '/api/employees/save'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .contentType("application/json")
                .body(" { " + 
                    " \"credential\": { " + 
                    " \"credentialId\": 1665453008, " + 
                    " \"password\": \"hOdfB__qZ\", " + 
                    " \"role\": \"IGK7ECsVr9\" " + 
                    " }, " + 
                    " \"email\": \"ILHw7m_bk\", " + 
                    " \"job\": \"WU1j6NtBol29z\", " + 
                    " \"lastName\": \"JEG\", " + 
                    " \"salary\": 0.551561401413652 " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/employees/save?password=")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", nullValue())
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-53"></a>
<details open>
<summary><b>test_53</b> &middot; F200 &middot; <code>PUT:/app/api/assignments/update</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/assignments/update
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_53() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/assignments/update -> Response status 400 not defined for path '/api/assignments/update'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .contentType("application/json")
                .body(" { " + 
                    " \"commitEmpDesc\": \"\", " + 
                    " \"projectId\": 78 " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/assignments/update?EMextraParam123=_EM_146_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("could not execute statement; SQL [n/a]; constraint [null]; nested exception is org.hibernate.exception.ConstraintViolationException: could not execute statement"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-54"></a>
<details open>
<summary><b>test_54</b> &middot; F200 &middot; <code>POST:/app/api/assignments</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/assignments
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_54() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/assignments -> Response status 400 not defined for path '/api/assignments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .contentType("application/json")
                .body(" { " + 
                    " \"commitMgrDesc\": \"_EM_373_XYZ_\", " + 
                    " \"employeeId\": 655, " + 
                    " \"projectId\": 3 " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/assignments")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("could not execute statement; SQL [n/a]; constraint [FK2_ASSIGN]; nested exception is org.hibernate.exception.ConstraintViolationException: could not execute statement"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-55"></a>
<details open>
<summary><b>test_55</b> &middot; F200 &middot; <code>GET:/app/api/assignments/data/project-commit/{projectId}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/assignments/data/project-commit/{projectId}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_55() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/data/project-commit/{projectId} -> Response status 400 not defined for path '/api/assignments/data/project-commit/{projectId}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .get(baseUrlOfSut + "/app/api/assignments/data/project-commit/_EM_1068_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"_EM_1068_XYZ_\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-56"></a>
<details open>
<summary><b>test_56</b> &middot; F200 &middot; <code>DELETE:/app/api/projects/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/projects/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_56() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/projects/{id} -> Response status 400 not defined for path '/api/projects/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .delete(baseUrlOfSut + "/app/api/projects/Qb3")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"Qb3\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-57"></a>
<details open>
<summary><b>test_57</b> &middot; F200 &middot; <code>GET:/app/api/locations/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/locations/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_57() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/locations/{id} -> Response status 400 not defined for path '/api/locations/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .get(baseUrlOfSut + "/app/api/locations/_EM_701_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"_EM_701_XYZ_\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-58"></a>
<details open>
<summary><b>test_58</b> &middot; F200 &middot; <code>PUT:/app/api/projects</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/projects
    * Found 1 potential fault of type-code 200
    * Using 1 example:
    *   dd-MM-yyyy
    */
    @Test @Timeout(60)
    public void test_58() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/projects -> Response status 400 not defined for path '/api/projects'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"endDate\": \"dd-MM-yyyy\", " + 
                    " \"startDate\": \"dd-MM-yyyy\", " + 
                    " \"title\": \"pkZsE6JebHQ\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/projects")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 12] (through reference chain: com.pfa.app.model.entity.Project[\"endDate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-59"></a>
<details open>
<summary><b>test_59</b> &middot; F200 &middot; <code>DELETE:/app/api/employees/username/{username}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/employees/username/{username}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_59() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/employees/username/{username} -> Response status 400 not defined for path '/api/employees/username/{username}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .delete(baseUrlOfSut + "/app/api/employees/username/0OH80Jdl4?username=xVKnegGAbts")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("###### NO Credential object FOUND with username: 0OH80Jdl4 ! ######"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-60"></a>
<details open>
<summary><b>test_60</b> &middot; F200 &middot; <code>POST:/app/api/projects/save</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/projects/save
    * Found 1 potential fault of type-code 200
    * Using 1 example:
    *   dd-MM-yyyy
    */
    @Test @Timeout(60)
    public void test_60() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/projects/save -> Response status 400 not defined for path '/api/projects/save'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"endDate\": \"_EM_811_XYZ_\", " + 
                    " \"projectId\": 628, " + 
                    " \"startDate\": \"dd-MM-yyyy\", " + 
                    " \"title\": \"1duKP3\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/projects/save")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"_EM_811_XYZ_\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text '_EM_811_XYZ_' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"_EM_811_XYZ_\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text '_EM_811_XYZ_' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 12] (through reference chain: com.pfa.app.model.entity.Project[\"endDate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-61"></a>
<details open>
<summary><b>test_61</b> &middot; F200 &middot; <code>POST:/app/api/projects</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/projects
    * Found 1 potential fault of type-code 200
    * Using 1 example:
    *   dd-MM-yyyy
    */
    @Test @Timeout(60)
    public void test_61() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/projects -> Response status 400 not defined for path '/api/projects'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"endDate\": \"dd-MM-yyyy\", " + 
                    " \"startDate\": \"hZYfkLoAy\", " + 
                    " \"title\": \"P0HJZLqdAh\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/projects")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 12] (through reference chain: com.pfa.app.model.entity.Project[\"endDate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-62"></a>
<details open>
<summary><b>test_62</b> &middot; F200 &middot; <code>DELETE:/app/api/employees/username/{username}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/employees/username/{username}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_62() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("LOCATIONS", 194L)
                .d("ADR", "\"w3H\"")
                .d("POSTAL_CODE", "\"Dm1wAxpyEMjb\"")
                .d("CITY", "\"8rd_w1ckvH\"")
            .and().insertInto("DEPARTMENTS", 193L)
                .d("DEPARTMENT_NAME", "\"7bX3sX_Met\"")
            .and().insertInto("EMPLOYEES", 192L)
                .d("FIRST_NAME", "\"My9G\"")
                .d("LAST_NAME", "\"RFHyTuEDtCE\"")
                .d("EMAIL", "\"uuv@Aof.zmB\"")
                .d("PHONE", "\"\"")
                .d("JOB", "\"Nj\"")
                .d("SALARY", "0.4694010292288521")
            .and().insertInto("LOCATIONS", 191L)
                .d("ADR", "\"P0ybfpv6F6KyJ\"")
                .d("POSTAL_CODE", "\"IN4RmVN7AjeJS\"")
                .d("CITY", "\"XQPrUjefS\"")
            .and().insertInto("DEPARTMENTS", 190L)
                .d("DEPARTMENT_NAME", "\"99N9DF1K1\"")
            .and().insertInto("EMPLOYEES", 189L)
                .d("FIRST_NAME", "\"FTXXY87mW_P\"")
                .d("LAST_NAME", "\"rk0hGRtCjItjXj\"")
                .d("EMAIL", "\"McOB@xou.VVp\"")
                .d("PHONE", "\"g_THHMqodiUzZ9S\"")
                .d("JOB", "\"bZl4fWx0\"")
                .d("SALARY", "0.43066421856502934")
            .and().insertInto("LOCATIONS", 188L)
                .d("ADR", "\"qPHW\"")
                .d("POSTAL_CODE", "\"xjG4V245l\"")
                .d("CITY", "\"0YjL3Si5Y\"")
            .and().insertInto("DEPARTMENTS", 187L)
                .d("DEPARTMENT_NAME", "\"k\"")
            .and().insertInto("EMPLOYEES", 186L)
                .d("FIRST_NAME", "\"QzA9YPfiA9j\"")
                .d("LAST_NAME", "\"D2cxNi\"")
                .d("EMAIL", "\"sZVV@niP.pN\"")
                .d("PHONE", "\"x9I5KwBc\"")
                .d("JOB", "\"VYqjGrja7\"")
                .d("SALARY", "0.5897441580772507")
            .and().insertInto("USER_CREDENTIALS", 185L)
                .d("USERNAME", "NULL")
                .d("PASSWORD", "\"0o2dGXZRFAligvW5\"")
                .d("ENABLED", "false")
                .d("ROLE", "\"1Cy6fJq4_CUPSH\"")
                .d("EMPLOYEE_ID", "NULL")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/employees/username/{username} -> Response status 400 not defined for path '/api/employees/username/{username}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .delete(baseUrlOfSut + "/app/api/employees/username/0OH80Jfl4?" + 
                    "password=KTzELGllTH&" + 
                    "username=xVKnegGAbts")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("###### NO Credential object FOUND with username: 0OH80Jfl4 ! ######"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-63"></a>
<details open>
<summary><b>test_63</b> &middot; F200 &middot; <code>GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}/{commitDate}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}/{commitDate}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_63() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}/{commitDate} -> Response status 400 not defined for path '/api/assignments/data/project-commit/{employeeId}/{projectId}/{commitDate}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .get(baseUrlOfSut + "/app/api/assignments/data/project-commit/eg6IX7JsGkzJqK/_EM_449_XYZ_/_EM_448_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"eg6IX7JsGkzJqK\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-64"></a>
<details open>
<summary><b>test_64</b> &middot; F200 &middot; <code>GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_64() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId} -> Response status 400 not defined for path '/api/assignments/data/project-commit/{employeeId}/{projectId}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .get(baseUrlOfSut + "/app/api/assignments/data/project-commit/1wD/oM9Sx?" + 
                    "password=BwvR_6c&" + 
                    "username=IOervlhojejjGBc0")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"1wD\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-65"></a>
<details open>
<summary><b>test_65</b> &middot; F200 &middot; <code>DELETE:/app/api/assignments/{employeeId}/{projectId}/{commitDate}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/assignments/{employeeId}/{projectId}/{commitDate}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_65() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/assignments/{employeeId}/{projectId}/{commitDate} -> Response status 400 not defined for path '/api/assignments/{employeeId}/{projectId}/{commitDate}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .delete(baseUrlOfSut + "/app/api/assignments/Gv/xEX0icafnWOHfF/19-12-202016:13:17")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"Gv\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-66"></a>
<details open>
<summary><b>test_66</b> &middot; F200 &middot; <code>GET:/app/api/employees/data/employee-project-data/{employeeId}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/employees/data/employee-project-data/{employeeId}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_66() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/employees/data/employee-project-data/{employeeId} -> Response status 400 not defined for path '/api/employees/data/employee-project-data/{employeeId}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .get(baseUrlOfSut + "/app/api/employees/data/employee-project-data/hSPpZnftGQUH?" + 
                    "password=&" + 
                    "username=VwSeKtqvu")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"hSPpZnftGQUH\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-67"></a>
<details open>
<summary><b>test_67</b> &middot; F200 &middot; <code>DELETE:/app/api/departments/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/departments/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_67() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/departments/{id} -> Response status 400 not defined for path '/api/departments/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .delete(baseUrlOfSut + "/app/api/departments/DIz")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"DIz\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-68"></a>
<details open>
<summary><b>test_68</b> &middot; F200 &middot; <code>DELETE:/app/api/locations/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/locations/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_68() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/locations/{id} -> Response status 400 not defined for path '/api/locations/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .delete(baseUrlOfSut + "/app/api/locations/9wto")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"9wto\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-69"></a>
<details open>
<summary><b>test_69</b> &middot; F200 &middot; <code>GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}/{commitDate}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}/{commitDate}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_69() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("DEPARTMENTS", 172L)
                .d("DEPARTMENT_NAME", "\"cpnXGmm\"")
            .and().insertInto("LOCATIONS", 167L)
                .d("ADR", "\"SeExk2L\"")
                .d("POSTAL_CODE", "\"bENRo6FTuZxueSZO\"")
                .d("CITY", "\"oD4qBBKgR76wmt\"")
            .and().insertInto("ASSIGNMENTS", 164L)
                .d("EMPLOYEE_ID", "13")
                .d("PROJECT_ID", "7")
                .d("COMMIT_DATE", "\"1965-05-04 06:17:30\"")
                .d("COMMIT_EMP_DESC", "\"oM\"")
                .d("COMMIT_MGR_DESC", "\"\"")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}/{commitDate} -> Response status 400 not defined for path '/api/assignments/data/project-commit/{employeeId}/{projectId}/{commitDate}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .get(baseUrlOfSut + "/app/api/assignments/data/project-commit/OWZrj_/4F86INwC_Cj/sqEN4qJpeBSNVa?" + 
                    "password=kYfkw0&" + 
                    "username=QN")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"OWZrj_\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-70"></a>
<details open>
<summary><b>test_70</b> &middot; F200 &middot; <code>GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}</code></summary>

```java
    /**
    * Calls:
    * (400) GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_70() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. GET:/app/api/assignments/data/project-commit/{employeeId}/{projectId} -> Response status 400 not defined for path '/api/assignments/data/project-commit/{employeeId}/{projectId}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .get(baseUrlOfSut + "/app/api/assignments/data/project-commit/z0m/oYcrH_89UgA66")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"z0m\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-71"></a>
<details open>
<summary><b>test_71</b> &middot; F200 &middot; <code>DELETE:/app/api/credentials/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/credentials/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_71() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/credentials/{id} -> Response status 400 not defined for path '/api/credentials/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .delete(baseUrlOfSut + "/app/api/credentials/_EM_476_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"_EM_476_XYZ_\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-72"></a>
<details open>
<summary><b>test_72</b> &middot; F200 &middot; <code>DELETE:/app/api/employees/delete/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/employees/delete/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_72() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/employees/delete/{id} -> Response status 400 not defined for path '/api/employees/delete/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .delete(baseUrlOfSut + "/app/api/employees/delete/_EM_469_XYZ_")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("For input string: \"_EM_469_XYZ_\""))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-73"></a>
<details open>
<summary><b>test_73</b> &middot; F200 &middot; <code>POST:/app/api/employees/save</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/employees/save
    * Found 1 potential fault of type-code 200
    * Using 1 example:
    *   dd-MM-yyyy
    */
    @Test @Timeout(60)
    public void test_73() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/employees/save -> Response status 400 not defined for path '/api/employees/save'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .contentType("application/json")
                .body(" { " + 
                    " \"email\": \"springabcxyzboot@gmail.com\", " + 
                    " \"hiredate\": \"dd-MM-yyyy\", " + 
                    " \"lastName\": \"zWQ2RTIRoyyDi\", " + 
                    " \"phone\": \"22125144\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/employees/save")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 51] (through reference chain: com.pfa.app.model.entity.Employee[\"hiredate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-74"></a>
<details open>
<summary><b>test_74</b> &middot; F200 &middot; <code>PUT:/app/api/projects/update</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/projects/update
    * Found 1 potential fault of type-code 200
    * Using 1 example:
    *   dd-MM-yyyy
    */
    @Test @Timeout(60)
    public void test_74() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/projects/update -> Response status 400 not defined for path '/api/projects/update'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .contentType("application/json")
                .body(" { " + 
                    " \"projectId\": 753, " + 
                    " \"startDate\": \"dd-MM-yyyy\", " + 
                    " \"status\": \"IN_PROGRESS\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/projects/update")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 31] (through reference chain: com.pfa.app.model.entity.Project[\"startDate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-75"></a>
<details open>
<summary><b>test_75</b> &middot; F200 &middot; <code>POST:/app/api/locations</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/locations
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_75() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/locations -> Response status 400 not defined for path '/api/locations'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" {} ")
                .post(baseUrlOfSut + "/app/api/locations")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Validation failed for classes [com.pfa.app.model.entity.Location] during persist time for groups [javax.validation.groups.Default, ]\nList of constraint violations:[\n\tConstraintViolationImpl{interpolatedMessage='*Must Not blank**', propertyPath=postalCode, rootBeanClass=class com.pfa.app.model.entity.Location, messageTemplate='*Must Not blank**'}\n\tConstraintViolationImpl{interpolatedMessage='*Must Not blank**', propertyPath=city, rootBeanClass=class com.pfa.app.model.entity.Location, messageTemplate='*Must Not blank**'}\n\tConstraintViolationImpl{interpolatedMessage='*Must Not blank**', propertyPath=adr, rootBeanClass=class com.pfa.app.model.entity.Location, messageTemplate='*Must Not blank**'}\n]"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-76"></a>
<details open>
<summary><b>test_76</b> &middot; F200 &middot; <code>POST:/app/api/assignments</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/assignments
    * Found 1 potential fault of type-code 200
    * Using 1 example:
    *   dd-MM-yyyyHH:mm:ss
    */
    @Test @Timeout(60)
    public void test_76() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/assignments -> Response status 400 not defined for path '/api/assignments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" { " + 
                    " \"commitDate\": \"dd-MM-yyyyHH:mm:ss\", " + 
                    " \"commitMgrDesc\": \"_EM_631_XYZ_\", " + 
                    " \"employeeId\": 666, " + 
                    " \"project\": { " + 
                    " \"projectId\": 9, " + 
                    " \"startDate\": \"9_\", " + 
                    " \"title\": \"_EM_634_XYZ_\" " + 
                    " }, " + 
                    " \"projectId\": 469 " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/assignments")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDateTime` from String \"dd-MM-yyyyHH:mm:ss\": Failed to deserialize java.time.LocalDateTime: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyyHH:mm:ss' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDateTime` from String \"dd-MM-yyyyHH:mm:ss\": Failed to deserialize java.time.LocalDateTime: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyyHH:mm:ss' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 15] (through reference chain: com.pfa.app.model.entity.Assignment[\"commitDate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-77"></a>
<details open>
<summary><b>test_77</b> &middot; F200 &middot; <code>PUT:/app/api/assignments/update</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/assignments/update
    * Found 1 potential fault of type-code 200
    * Using 1 example:
    *   dd-MM-yyyy
    */
    @Test @Timeout(60)
    public void test_77() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/assignments/update -> Response status 400 not defined for path '/api/assignments/update'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .contentType("application/json")
                .body(" { " + 
                    " \"commitDate\": \"jGOTiv5k\", " + 
                    " \"commitMgrDesc\": \"qu2r\", " + 
                    " \"employee\": { " + 
                    " \"department\": { " + 
                    " \"departmentName\": \"Digital\", " + 
                    " \"location\": { " + 
                    " \"city\": \"3ady1Mpa\", " + 
                    " \"postalCode\": \"\" " + 
                    " } " + 
                    " }, " + 
                    " \"email\": \"_EM_1047_XYZ_\", " + 
                    " \"firstName\": \"gB7szWN4\", " + 
                    " \"hiredate\": \"dd-MM-yyyy\", " + 
                    " \"job\": \"OjcdSk\" " + 
                    " }, " + 
                    " \"project\": { " + 
                    " \"endDate\": \"7\", " + 
                    " \"projectId\": 5 " + 
                    " }, " + 
                    " \"projectId\": 3 " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/assignments/update")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDateTime` from String \"jGOTiv5k\": Failed to deserialize java.time.LocalDateTime: (java.time.format.DateTimeParseException) Text 'jGOTiv5k' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDateTime` from String \"jGOTiv5k\": Failed to deserialize java.time.LocalDateTime: (java.time.format.DateTimeParseException) Text 'jGOTiv5k' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 15] (through reference chain: com.pfa.app.model.entity.Assignment[\"commitDate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-78"></a>
<details open>
<summary><b>test_78</b> &middot; F200 &middot; <code>POST:/app/api/assignments/save</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/assignments/save
    * Found 1 potential fault of type-code 200
    * Using 2 examples:
    *   dd-MM-yyyy
    *   dd-MM-yyyyHH:mm:ss
    */
    @Test @Timeout(60)
    public void test_78() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/assignments/save -> Response status 400 not defined for path '/api/assignments/save'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .contentType("application/json")
                .body(" { " + 
                    " \"commitDate\": \"dd-MM-yyyyHH:mm:ss\", " + 
                    " \"commitEmpDesc\": \"8VE\", " + 
                    " \"employee\": { " + 
                    " \"department\": { " + 
                    " \"location\": { " + 
                    " \"city\": \"_FxO6dv6KTq\", " + 
                    " \"locationId\": 167 " + 
                    " } " + 
                    " }, " + 
                    " \"hiredate\": \"dd-MM-yyyy\", " + 
                    " \"job\": \"_EM_1030_XYZ_\", " + 
                    " \"lastName\": \"x9Es5Sthot\" " + 
                    " }, " + 
                    " \"employeeId\": 68 " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/assignments/save")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDateTime` from String \"dd-MM-yyyyHH:mm:ss\": Failed to deserialize java.time.LocalDateTime: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyyHH:mm:ss' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDateTime` from String \"dd-MM-yyyyHH:mm:ss\": Failed to deserialize java.time.LocalDateTime: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyyHH:mm:ss' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 15] (through reference chain: com.pfa.app.model.entity.Assignment[\"commitDate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-79"></a>
<details open>
<summary><b>test_79</b> &middot; F200 &middot; <code>POST:/app/api/departments</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/departments
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_79() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/departments -> Response status 400 not defined for path '/api/departments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" {} ")
                .post(baseUrlOfSut + "/app/api/departments")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Validation failed for classes [com.pfa.app.model.entity.Department] during persist time for groups [javax.validation.groups.Default, ]\nList of constraint violations:[\n\tConstraintViolationImpl{interpolatedMessage='*Must not blank**', propertyPath=departmentName, rootBeanClass=class com.pfa.app.model.entity.Department, messageTemplate='*Must not blank**'}\n\tConstraintViolationImpl{interpolatedMessage='*Must not NULL**', propertyPath=location, rootBeanClass=class com.pfa.app.model.entity.Department, messageTemplate='*Must not NULL**'}\n]"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-80"></a>
<details open>
<summary><b>test_80</b> &middot; F200 &middot; <code>POST:/app/api/assignments</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/assignments
    * Found 1 potential fault of type-code 200
    * Using 1 example:
    *   dd-MM-yyyy
    */
    @Test @Timeout(60)
    public void test_80() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/assignments -> Response status 400 not defined for path '/api/assignments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .contentType("application/json")
                .body(" { " + 
                    " \"commitDate\": \"I0ZCwTo\", " + 
                    " \"employee\": { " + 
                    " \"credential\": { " + 
                    " \"enabled\": false, " + 
                    " \"role\": \"42Xcf5NeLLjHM6VN\" " + 
                    " }, " + 
                    " \"email\": \"77ms\", " + 
                    " \"employeeId\": 5, " + 
                    " \"job\": \"Chef service Billing\", " + 
                    " \"lastName\": \"4gtOK\", " + 
                    " \"salary\": 0.05239085058550608 " + 
                    " }, " + 
                    " \"employeeId\": 419, " + 
                    " \"project\": { " + 
                    " \"endDate\": \"dd-MM-yyyy\", " + 
                    " \"startDate\": \"dd-MM-yyyy\", " + 
                    " \"title\": \"5Bw4dS8lw6Ix_h\" " + 
                    " }, " + 
                    " \"projectId\": 69 " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/assignments")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDateTime` from String \"I0ZCwTo\": Failed to deserialize java.time.LocalDateTime: (java.time.format.DateTimeParseException) Text 'I0ZCwTo' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDateTime` from String \"I0ZCwTo\": Failed to deserialize java.time.LocalDateTime: (java.time.format.DateTimeParseException) Text 'I0ZCwTo' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 15] (through reference chain: com.pfa.app.model.entity.Assignment[\"commitDate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-81"></a>
<details open>
<summary><b>test_81</b> &middot; F200 &middot; <code>PUT:/app/api/credentials</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/credentials
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_81() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/credentials -> Response status 400 not defined for path '/api/credentials'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" { " + 
                    " \"username\": \"7B_1xnA6\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/credentials")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("rawPassword cannot be null"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-82"></a>
<details open>
<summary><b>test_82</b> &middot; F200 &middot; <code>PUT:/app/api/projects/update</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/projects/update
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_82() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/projects/update -> Response status 400 not defined for path '/api/projects/update'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"status\": \"T\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/projects/update")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Validation failed for classes [com.pfa.app.model.entity.Project] during persist time for groups [javax.validation.groups.Default, ]\nList of constraint violations:[\n\tConstraintViolationImpl{interpolatedMessage='Must not blank*', propertyPath=title, rootBeanClass=class com.pfa.app.model.entity.Project, messageTemplate='Must not blank*'}\n]"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-83"></a>
<details open>
<summary><b>test_83</b> &middot; F200 &middot; <code>PUT:/app/api/projects</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/projects
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_83() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/projects -> Response status 400 not defined for path '/api/projects'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"status\": \"csQ_xm8ovT\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/projects")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Validation failed for classes [com.pfa.app.model.entity.Project] during persist time for groups [javax.validation.groups.Default, ]\nList of constraint violations:[\n\tConstraintViolationImpl{interpolatedMessage='Must not blank*', propertyPath=title, rootBeanClass=class com.pfa.app.model.entity.Project, messageTemplate='Must not blank*'}\n]"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-84"></a>
<details open>
<summary><b>test_84</b> &middot; F200 &middot; <code>POST:/app/api/departments/save</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/departments/save
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_84() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/departments/save -> Response status 400 not defined for path '/api/departments/save'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" { " + 
                    " \"departmentId\": 1, " + 
                    " \"departmentName\": \"M1rLB5\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/departments/save")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Validation failed for classes [com.pfa.app.model.entity.Department] during persist time for groups [javax.validation.groups.Default, ]\nList of constraint violations:[\n\tConstraintViolationImpl{interpolatedMessage='*Must not NULL**', propertyPath=location, rootBeanClass=class com.pfa.app.model.entity.Department, messageTemplate='*Must not NULL**'}\n]"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-85"></a>
<details open>
<summary><b>test_85</b> &middot; F200 &middot; <code>PUT:/app/api/departments/update</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/departments/update
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_85() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/departments/update -> Response status 400 not defined for path '/api/departments/update'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"departmentId\": 258, " + 
                    " \"departmentName\": \"Rwiu\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/departments/update?username=CwlZMZZr9U5h8")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Validation failed for classes [com.pfa.app.model.entity.Department] during persist time for groups [javax.validation.groups.Default, ]\nList of constraint violations:[\n\tConstraintViolationImpl{interpolatedMessage='*Must not NULL**', propertyPath=location, rootBeanClass=class com.pfa.app.model.entity.Department, messageTemplate='*Must not NULL**'}\n]"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-86"></a>
<details open>
<summary><b>test_86</b> &middot; F200 &middot; <code>PUT:/app/api/departments/update</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/departments/update
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_86() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("LOCATIONS", 121L)
                .d("ADR", "\"5rSSv1SVBt73CSj\"")
                .d("POSTAL_CODE", "\"47HK8SLbBj8VZ\"")
                .d("CITY", "\"xbfnDGUTzMtfH9wY\"")
            .and().insertInto("DEPARTMENTS", 120L)
                .d("DEPARTMENT_NAME", "\"9wyDtz72G9Kibn6\"")
                .d("LOCATION_ID", "NULL")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/departments/update -> Response status 400 not defined for path '/api/departments/update'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"departmentId\": 258, " + 
                    " \"departmentName\": \"Rwiu\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/departments/update?" + 
                    "password=qfT2oU6&" + 
                    "username=CwlZMZZr8U5h8")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Validation failed for classes [com.pfa.app.model.entity.Department] during persist time for groups [javax.validation.groups.Default, ]\nList of constraint violations:[\n\tConstraintViolationImpl{interpolatedMessage='*Must not NULL**', propertyPath=location, rootBeanClass=class com.pfa.app.model.entity.Department, messageTemplate='*Must not NULL**'}\n]"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-87"></a>
<details open>
<summary><b>test_87</b> &middot; F200 &middot; <code>POST:/app/api/credentials/save</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/credentials/save
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_87() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/credentials/save -> Response status 400 not defined for path '/api/credentials/save'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"credentialId\": 620, " + 
                    " \"password\": \"Nutm\", " + 
                    " \"role\": \"HEbdBH\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/credentials/save")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("could not execute statement; SQL [n/a]; constraint [null]; nested exception is org.hibernate.exception.ConstraintViolationException: could not execute statement"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-88"></a>
<details open>
<summary><b>test_88</b> &middot; F200 &middot; <code>PUT:/app/api/credentials/update</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/credentials/update
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_88() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/credentials/update -> Response status 400 not defined for path '/api/credentials/update'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" { " + 
                    " \"credentialId\": 123, " + 
                    " \"enabled\": false, " + 
                    " \"role\": \"uf3aruhEMZAkS\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/credentials/update")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("rawPassword cannot be null"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-89"></a>
<details open>
<summary><b>test_89</b> &middot; F200 &middot; <code>POST:/app/api/assignments</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/assignments
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_89() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/assignments -> Response status 400 not defined for path '/api/assignments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "42")
                .contentType("application/json")
                .body(" { " + 
                    " \"commitMgrDesc\": \"kX4T\", " + 
                    " \"employeeId\": 999, " + 
                    " \"project\": { " + 
                    " \"endDate\": \"\", " + 
                    " \"title\": \"SYNCH_BSCS_IMX\" " + 
                    " }, " + 
                    " \"projectId\": 6 " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/assignments")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("org.hibernate.TransientPropertyValueException: Not-null property references a transient value - transient instance must be saved before current operation : com.pfa.app.model.entity.Assignment.project -> com.pfa.app.model.entity.Project; nested exception is java.lang.IllegalStateException: org.hibernate.TransientPropertyValueException: Not-null property references a transient value - transient instance must be saved before current operation : com.pfa.app.model.entity.Assignment.project -> com.pfa.app.model.entity.Project"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-90"></a>
<details open>
<summary><b>test_90</b> &middot; F200 &middot; <code>PUT:/app/api/departments/update</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/departments/update
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_90() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/departments/update -> Response status 400 not defined for path '/api/departments/update'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" { " + 
                    " \"departmentId\": 1 " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/departments/update")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Could not commit JPA transaction; nested exception is javax.persistence.RollbackException: Error while committing the transaction"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-91"></a>
<details open>
<summary><b>test_91</b> &middot; F200 &middot; <code>DELETE:/app/api/credentials/{id}</code></summary>

```java
    /**
    * Calls:
    * (400) DELETE:/app/api/credentials/{id}
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_91() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. DELETE:/app/api/credentials/{id} -> Response status 400 not defined for path '/api/credentials/{id}'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .delete(baseUrlOfSut + "/app/api/credentials/6")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("could not execute statement; SQL [n/a]; constraint [\"FK2_EMP: PUBLIC.EMPLOYEES FOREIGN KEY(MANAGER_ID) REFERENCES PUBLIC.EMPLOYEES(EMPLOYEE_ID) (5)\"; SQL statement:\n/* delete com.pfa.app.model.entity.Employee */ delete from employees where employee_id=? [23503-200]]; nested exception is org.hibernate.exception.ConstraintViolationException: could not execute statement"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-92"></a>
<details open>
<summary><b>test_92</b> &middot; F200 &middot; <code>POST:/app/api/employees</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/employees
    * Found 1 potential fault of type-code 200
    * Using 1 example:
    *   dd-MM-yyyy
    */
    @Test @Timeout(60)
    public void test_92() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/employees -> Response status 400 not defined for path '/api/employees'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .contentType("application/json")
                .body(" { " + 
                    " \"credential\": { " + 
                    " \"credentialId\": 638, " + 
                    " \"enabled\": true, " + 
                    " \"password\": \"r\", " + 
                    " \"role\": \"m4GiSzsPuZr0TEp\" " + 
                    " }, " + 
                    " \"firstName\": \"QukZDeqlUW\", " + 
                    " \"hiredate\": \"dd-MM-yyyy\", " + 
                    " \"lastName\": \"uN7\", " + 
                    " \"phone\": \"NTNR8XPGZ0OBZn\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/employees?" + 
                    "password=&" + 
                    "username=cqD3ahZpx")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 132] (through reference chain: com.pfa.app.model.entity.Employee[\"hiredate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-93"></a>
<details open>
<summary><b>test_93</b> &middot; F200 &middot; <code>POST:/app/api/locations</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/locations
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_93() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/locations -> Response status 400 not defined for path '/api/locations'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" { " + 
                    " \"adr\": \"RUE DE LA BOURSE\", " + 
                    " \"city\": \"_EM_699_XYZ_\", " + 
                    " \"locationId\": 465, " + 
                    " \"postalCode\": \"_EM_700_XYZ_\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/locations")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("could not execute statement; SQL [n/a]; constraint [\"PRIMARY KEY ON PUBLIC.LOCATIONS(LOCATION_ID) [2, 'RUE DE BLA BLA', '2016', 'CHARGUIA']\"; SQL statement:\n/* insert com.pfa.app.model.entity.Location */ insert into locations (location_id, adr, city, postal_code) values (null, ?, ?, ?) [23505-200]]; nested exception is org.hibernate.exception.ConstraintViolationException: could not execute statement"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-94"></a>
<details open>
<summary><b>test_94</b> &middot; F200 &middot; <code>POST:/app/api/authenticate/</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/authenticate/
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_94() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("LOCATIONS", 184L)
                .d("ADR", "\"6G4D98tyi9LRCVRH\"")
                .d("POSTAL_CODE", "\"IJxkZcr2XNPDwRe\"")
                .d("CITY", "\"9mzdskyz1hyfKbDd\"")
            .and().insertInto("DEPARTMENTS", 183L)
                .d("DEPARTMENT_NAME", "\"ERq0VnVRo0THPs\"")
            .and().insertInto("EMPLOYEES", 182L)
                .d("FIRST_NAME", "\"Z\"")
                .d("LAST_NAME", "\"slw5wjaO\"")
                .d("EMAIL", "\"OaFw@oD.fk\"")
                .d("PHONE", "\"YyZ6X4uiMyKllzlS\"")
                .d("JOB", "\"r\"")
                .d("SALARY", "0.8041016092143625")
            .and().insertInto("EMPLOYEES", 179L)
                .d("FIRST_NAME", "\"sLJ\"")
                .d("LAST_NAME", "\"PtQM0s4f4GfN\"")
                .d("EMAIL", "\"kDSv@Obp.DCTe\"")
                .d("PHONE", "\"Y7ksmtGOKO1J\"")
                .d("JOB", "\"IQs9kcSRW23C\"")
                .d("SALARY", "0.8644621741318967")
            .and().insertInto("USER_CREDENTIALS", 175L)
                .d("USERNAME", "\"0uU\"")
                .d("PASSWORD", "\"2\"")
                .d("ENABLED", "false")
                .d("ROLE", "\"Xf1JktFaQTEt3g\"")
                .d("EMPLOYEE_ID", "NULL")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/authenticate/ -> Response status 400 not defined for path '/api/authenticate/'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"username\": \"8aPcf5fiNbqq\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/authenticate/")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Bad credentials"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-95"></a>
<details open>
<summary><b>test_95</b> &middot; F200 &middot; <code>PUT:/app/api/projects</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/projects
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_95() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/projects -> Response status 400 not defined for path '/api/projects'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"projectId\": 817, " + 
                    " \"startDate\": \"29-01-2021\", " + 
                    " \"status\": \"AOKW11N\", " + 
                    " \"title\": \"Niu4TlzpIU\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/projects")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("could not execute statement; SQL [n/a]; constraint [\"PRIMARY KEY ON PUBLIC.PROJECTS(PROJECT_ID) [1, 'TRANSBSCS', DATE '2020-09-28', DATE '2020-11-04', 'COMPLETED']\"; SQL statement:\n/* insert com.pfa.app.model.entity.Project */ insert into projects (project_id, end_date, start_date, status, title) values (null, ?, ?, ?, ?) [23505-200]]; nested exception is org.hibernate.exception.ConstraintViolationException: could not execute statement"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-96"></a>
<details open>
<summary><b>test_96</b> &middot; F200 &middot; <code>PUT:/app/api/locations/update</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/locations/update
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_96() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/locations/update -> Response status 400 not defined for path '/api/locations/update'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" { " + 
                    " \"adr\": \"RUE DE LA BOURSE\", " + 
                    " \"city\": \"xpfSAmJjiJU7\", " + 
                    " \"locationId\": 908, " + 
                    " \"postalCode\": \"FVuCCsLyZ4L\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/locations/update")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("could not execute statement; SQL [n/a]; constraint [\"PRIMARY KEY ON PUBLIC.LOCATIONS(LOCATION_ID) [2, 'RUE DE BLA BLA', '2016', 'CHARGUIA']\"; SQL statement:\n/* insert com.pfa.app.model.entity.Location */ insert into locations (location_id, adr, city, postal_code) values (null, ?, ?, ?) [23505-200]]; nested exception is org.hibernate.exception.ConstraintViolationException: could not execute statement"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-97"></a>
<details open>
<summary><b>test_97</b> &middot; F200 &middot; <code>POST:/app/api/authenticate/</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/authenticate/
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_97() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("LOCATIONS", 184L)
                .d("ADR", "\"6G4D98tyi9LRCVRH\"")
                .d("POSTAL_CODE", "\"IJxkZcr2XNPDwRe\"")
                .d("CITY", "\"9mzdskyz1hyfKbDd\"")
            .and().insertInto("DEPARTMENTS", 183L)
                .d("DEPARTMENT_NAME", "\"ERq0VnVRo0THPs\"")
            .and().insertInto("EMPLOYEES", 182L)
                .d("FIRST_NAME", "\"Z\"")
                .d("LAST_NAME", "\"slw5wjaO\"")
                .d("EMAIL", "\"OaFw@oD.fk\"")
                .d("PHONE", "\"YyZ6X4uiMyKllzlS\"")
                .d("JOB", "\"r\"")
                .d("SALARY", "0.8041016092143625")
            .and().insertInto("EMPLOYEES", 179L)
                .d("FIRST_NAME", "\"sLJ\"")
                .d("LAST_NAME", "\"PtQM0s4f4GfN\"")
                .d("EMAIL", "\"kDSv@Obp.DCTe\"")
                .d("PHONE", "\"Y7ksmtGOKO1J\"")
                .d("JOB", "\"IQs9kcSRW23C\"")
                .d("SALARY", "0.8644621741318967")
            .and().insertInto("USER_CREDENTIALS", 175L)
                .d("USERNAME", "\"0uU\"")
                .d("PASSWORD", "\"2\"")
                .d("ENABLED", "false")
                .d("ROLE", "\"Xf1JktFaQTEt3g\"")
                .d("EMPLOYEE_ID", "5")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/authenticate/ -> Response status 400 not defined for path '/api/authenticate/'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"username\": \"8aPcf5fiNbqq\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/authenticate/?" + 
                    "password=m8qYgPY&" + 
                    "username=")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Bad credentials"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-98"></a>
<details open>
<summary><b>test_98</b> &middot; F200 &middot; <code>POST:/app/api/assignments/save</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/assignments/save
    * Found 1 potential fault of type-code 200
    * Using 1 example:
    *   dd-MM-yyyy
    */
    @Test @Timeout(60)
    public void test_98() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/assignments/save -> Response status 400 not defined for path '/api/assignments/save'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" { " + 
                    " \"commitDate\": \"12-12-202016:43:48\", " + 
                    " \"commitEmpDesc\": \"_EM_494_XYZ_\", " + 
                    " \"commitMgrDesc\": \"you need to implement sec solution\", " + 
                    " \"employee\": { " + 
                    " \"email\": \"KL1Lpdtux\", " + 
                    " \"employeeId\": 970, " + 
                    " \"hiredate\": \"d1qRqRP0S\", " + 
                    " \"lastName\": \"g4xo547\", " + 
                    " \"phone\": \"_EM_497_XYZ_\", " + 
                    " \"salary\": 0.06578326796072143 " + 
                    " }, " + 
                    " \"employeeId\": 551, " + 
                    " \"project\": { " + 
                    " \"endDate\": \"\", " + 
                    " \"projectId\": 490, " + 
                    " \"startDate\": \"dd-MM-yyyy\", " + 
                    " \"status\": \"_EM_498_XYZ_\", " + 
                    " \"title\": \"Jyv_HSYdLkl4btz\" " + 
                    " } " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/assignments/save")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"d1qRqRP0S\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'd1qRqRP0S' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"d1qRqRP0S\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'd1qRqRP0S' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 185] (through reference chain: com.pfa.app.model.entity.Assignment[\"employee\"]->com.pfa.app.model.entity.Employee[\"hiredate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-99"></a>
<details open>
<summary><b>test_99</b> &middot; F200 &middot; <code>PUT:/app/api/departments</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/departments
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_99() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/departments -> Response status 400 not defined for path '/api/departments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"departmentName\": \"SXdINjRKnc\", " + 
                    " \"location\": { " + 
                    " \"locationId\": 299, " + 
                    " \"postalCode\": \"fYmB\" " + 
                    " } " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/departments")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("could not execute statement; SQL [n/a]; constraint [FK1_DEPT]; nested exception is org.hibernate.exception.ConstraintViolationException: could not execute statement"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-100"></a>
<details open>
<summary><b>test_100</b> &middot; F200 &middot; <code>PUT:/app/api/assignments/update</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/assignments/update
    * Found 1 potential fault of type-code 200
    * Using 1 example:
    *   dd-MM-yyyy
    */
    @Test @Timeout(60)
    public void test_100() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/assignments/update -> Response status 400 not defined for path '/api/assignments/update'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .contentType("application/json")
                .body(" { " + 
                    " \"commitEmpDesc\": \"AK\", " + 
                    " \"commitMgrDesc\": \"AK\", " + 
                    " \"employee\": { " + 
                    " \"email\": \"\", " + 
                    " \"employeeId\": 280, " + 
                    " \"firstName\": \"ejtbu_\", " + 
                    " \"hiredate\": \"kut_o965Dz5byr\", " + 
                    " \"job\": \"x\", " + 
                    " \"salary\": 0.5090050256472601 " + 
                    " }, " + 
                    " \"employeeId\": 404, " + 
                    " \"project\": { " + 
                    " \"endDate\": \"\", " + 
                    " \"projectId\": 228, " + 
                    " \"startDate\": \"dd-MM-yyyy\", " + 
                    " \"status\": \"_EM_1087_XYZ_\", " + 
                    " \"title\": \"v5KXF2of1Gw468A\" " + 
                    " }, " + 
                    " \"projectId\": 986 " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/assignments/update")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"kut_o965Dz5byr\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'kut_o965Dz5byr' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"kut_o965Dz5byr\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'kut_o965Dz5byr' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 121] (through reference chain: com.pfa.app.model.entity.Assignment[\"employee\"]->com.pfa.app.model.entity.Employee[\"hiredate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-101"></a>
<details open>
<summary><b>test_101</b> &middot; F200 &middot; <code>POST:/app/api/assignments</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/assignments
    * Found 1 potential fault of type-code 200
    * Using 1 example:
    *   dd-MM-yyyy
    */
    @Test @Timeout(60)
    public void test_101() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/assignments -> Response status 400 not defined for path '/api/assignments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"commitMgrDesc\": \"ShHKh0k6vPvnPdqH\", " + 
                    " \"employee\": { " + 
                    " \"credential\": {}, " + 
                    " \"department\": { " + 
                    " \"location\": {} " + 
                    " }, " + 
                    " \"email\": \"puOlRHrzoy\", " + 
                    " \"hiredate\": \"dd-MM-yyyy\", " + 
                    " \"lastName\": \"MWviXI4zYMuWNf9\", " + 
                    " \"phone\": \"aWtvlRK\" " + 
                    " }, " + 
                    " \"employeeId\": 675 " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/assignments")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"dd-MM-yyyy\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'dd-MM-yyyy' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 130] (through reference chain: com.pfa.app.model.entity.Assignment[\"employee\"]->com.pfa.app.model.entity.Employee[\"hiredate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-102"></a>
<details open>
<summary><b>test_102</b> &middot; F200 &middot; <code>PUT:/app/api/locations</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/locations
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_102() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/locations -> Response status 400 not defined for path '/api/locations'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"adr\": \"_EM_867_XYZ_\", " + 
                    " \"locationId\": 2, " + 
                    " \"postalCode\": \"YC7E\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/locations")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Could not commit JPA transaction; nested exception is javax.persistence.RollbackException: Error while committing the transaction"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-103"></a>
<details open>
<summary><b>test_103</b> &middot; F200 &middot; <code>POST:/app/api/departments/save</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/departments/save
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_103() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/departments/save -> Response status 400 not defined for path '/api/departments/save'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"departmentName\": \"743ZkqUW\", " + 
                    " \"location\": { " + 
                    " \"city\": \"sqnDVgM6Hf\", " + 
                    " \"locationId\": 866, " + 
                    " \"postalCode\": \"F6f\" " + 
                    " } " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/departments/save")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("could not execute statement; SQL [n/a]; constraint [FK1_DEPT]; nested exception is org.hibernate.exception.ConstraintViolationException: could not execute statement"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-104"></a>
<details open>
<summary><b>test_104</b> &middot; F200 &middot; <code>POST:/app/api/projects</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/projects
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_104() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/projects -> Response status 400 not defined for path '/api/projects'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .contentType("application/json")
                .body(" { " + 
                    " \"projectId\": 9 " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/projects")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Could not commit JPA transaction; nested exception is javax.persistence.RollbackException: Error while committing the transaction"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-105"></a>
<details open>
<summary><b>test_105</b> &middot; F200 &middot; <code>POST:/app/api/assignments</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/assignments
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_105() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/assignments -> Response status 400 not defined for path '/api/assignments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .contentType("application/json")
                .body(" { " + 
                    " \"commitDate\": \"12-12-202015:10:28\", " + 
                    " \"employee\": { " + 
                    " \"job\": \"_EM_387_XYZ_\", " + 
                    " \"salary\": 0.6035240934929194 " + 
                    " }, " + 
                    " \"employeeId\": 183, " + 
                    " \"project\": { " + 
                    " \"endDate\": \"04-11-2020\", " + 
                    " \"status\": \"f\" " + 
                    " } " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/assignments")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("org.hibernate.TransientPropertyValueException: Not-null property references a transient value - transient instance must be saved before current operation : com.pfa.app.model.entity.Assignment.employee -> com.pfa.app.model.entity.Employee; nested exception is java.lang.IllegalStateException: org.hibernate.TransientPropertyValueException: Not-null property references a transient value - transient instance must be saved before current operation : com.pfa.app.model.entity.Assignment.employee -> com.pfa.app.model.entity.Employee"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-106"></a>
<details open>
<summary><b>test_106</b> &middot; F200 &middot; <code>POST:/app/api/departments</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/departments
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_106() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/departments -> Response status 400 not defined for path '/api/departments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" { " + 
                    " \"departmentId\": 4, " + 
                    " \"departmentName\": \"pTDhLagW2G79mV\", " + 
                    " \"location\": { " + 
                    " \"adr\": \"KskXldkyZ\", " + 
                    " \"postalCode\": \"zrH\" " + 
                    " } " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/departments")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("org.hibernate.TransientPropertyValueException: object references an unsaved transient instance - save the transient instance before flushing : com.pfa.app.model.entity.Department.location -> com.pfa.app.model.entity.Location; nested exception is java.lang.IllegalStateException: org.hibernate.TransientPropertyValueException: object references an unsaved transient instance - save the transient instance before flushing : com.pfa.app.model.entity.Department.location -> com.pfa.app.model.entity.Location"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-107"></a>
<details open>
<summary><b>test_107</b> &middot; F200 &middot; <code>POST:/app/api/assignments</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/assignments
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_107() throws Exception {
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/assignments -> Response status 400 not defined for path '/api/assignments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .contentType("application/json")
                .body(" { " + 
                    " \"commitEmpDesc\": \"3nYr9XOcbBqJ\", " + 
                    " \"employee\": { " + 
                    " \"credential\": { " + 
                    " \"password\": \"arf8zd_\", " + 
                    " \"role\": \"ZKP8TwWRP4Lsa_w\" " + 
                    " }, " + 
                    " \"department\": { " + 
                    " \"departmentName\": \"gTPQ\", " + 
                    " \"location\": { " + 
                    " \"locationId\": 994 " + 
                    " } " + 
                    " }, " + 
                    " \"email\": \"qCiMPKQSRwE\", " + 
                    " \"firstName\": \"\", " + 
                    " \"hiredate\": \"UERVgHEwCBM9mvR\", " + 
                    " \"job\": \"bSPAId0R\", " + 
                    " \"lastName\": \"IB1x\", " + 
                    " \"phone\": \"vV8y\" " + 
                    " }, " + 
                    " \"employeeId\": 957, " + 
                    " \"project\": { " + 
                    " \"endDate\": \"CSOl4tHVcolb\" " + 
                    " }, " + 
                    " \"projectId\": 319 " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/assignments?" + 
                    "password=NLwZZDt6D_dppu&" + 
                    "username=FHUP078Y")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("JSON parse error: Cannot deserialize value of type `java.time.LocalDate` from String \"UERVgHEwCBM9mvR\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'UERVgHEwCBM9mvR' could not be parsed at index 0; nested exception is com.fasterxml.jackson.databind.exc.InvalidFormatException: Cannot deserialize value of type `java.time.LocalDate` from String \"UERVgHEwCBM9mvR\": Failed to deserialize java.time.LocalDate: (java.time.format.DateTimeParseException) Text 'UERVgHEwCBM9mvR' could not be parsed at index 0\n at [Source: (ByteArrayInputStream); line: 1, column: 230] (through reference chain: com.pfa.app.model.entity.Assignment[\"employee\"]->com.pfa.app.model.entity.Employee[\"hiredate\"])"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-108"></a>
<details open>
<summary><b>test_108</b> &middot; F200 &middot; <code>PUT:/app/api/assignments</code></summary>

```java
    /**
    * Calls:
    * (400) PUT:/app/api/assignments
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_108() throws Exception {
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. PUT:/app/api/assignments -> Response status 400 not defined for path '/api/assignments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .contentType("application/json")
                .body(" { " + 
                    " \"commitEmpDesc\": \"_EM_167_XYZ_\", " + 
                    " \"commitMgrDesc\": \"_EM_168_XYZ_\", " + 
                    " \"employee\": { " + 
                    " \"credential\": { " + 
                    " \"credentialId\": 230, " + 
                    " \"enabled\": true, " + 
                    " \"password\": \"_EM_169_XYZ_\", " + 
                    " \"username\": \"_BZRksp\" " + 
                    " }, " + 
                    " \"employeeId\": 844, " + 
                    " \"lastName\": \"Tlemseni\", " + 
                    " \"salary\": 0.4894450152136409 " + 
                    " }, " + 
                    " \"employeeId\": 14, " + 
                    " \"project\": { " + 
                    " \"projectId\": 560, " + 
                    " \"status\": \"_EM_175_XYZ_\" " + 
                    " }, " + 
                    " \"projectId\": 873 " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/assignments")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("Unable to find com.pfa.app.model.entity.Employee with id 844; nested exception is javax.persistence.EntityNotFoundException: Unable to find com.pfa.app.model.entity.Employee with id 844"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-faults-java-test-109"></a>
<details open>
<summary><b>test_109</b> &middot; F200 &middot; <code>POST:/app/api/assignments</code></summary>

```java
    /**
    * Calls:
    * (400) POST:/app/api/assignments
    * Found 1 potential fault of type-code 200
    */
    @Test @Timeout(60)
    public void test_109() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        // Fault200. Received A Response From API That Is Not Valid According To Its Schema. POST:/app/api/assignments -> Response status 400 not defined for path '/api/assignments'.
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" { " + 
                    " \"commitMgrDesc\": \"h6c2gObl\", " + 
                    " \"employee\": { " + 
                    " \"credential\": { " + 
                    " \"credentialId\": 837, " + 
                    " \"password\": \"fmr2j\" " + 
                    " }, " + 
                    " \"department\": { " + 
                    " \"departmentId\": 604, " + 
                    " \"departmentName\": \"_EM_532_XYZ_\" " + 
                    " }, " + 
                    " \"hiredate\": \"01-01-2559\", " + 
                    " \"job\": \"_EM_536_XYZ_\", " + 
                    " \"phone\": \"22125144\" " + 
                    " } " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/assignments")
                .then()
                .statusCode(400)
                .assertThat()
                .contentType("application/json")
                .body("'msg'", containsString("org.hibernate.TransientPropertyValueException: Not-null property references a transient value - transient instance must be saved before current operation : com.pfa.app.model.entity.Assignment.employee -> com.pfa.app.model.entity.Employee; nested exception is java.lang.IllegalStateException: org.hibernate.TransientPropertyValueException: Not-null property references a transient value - transient instance must be saved before current operation : com.pfa.app.model.entity.Assignment.employee -> com.pfa.app.model.entity.Employee"))
                .body("'status'", containsString("BAD_REQUEST"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

#### successes.java (17)

<a name="test-successes-java-test-0"></a>
<details open>
<summary><b>test_0</b></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/v2/api-docs
    */
    @Test @Timeout(60)
    public void test_0() throws Exception {
        
        given().accept("*/*")
                .get(baseUrlOfSut + "/app/v2/api-docs")
                .then()
                .statusCode(200);
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-1"></a>
<details open>
<summary><b>test_1</b></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/projects/
    */
    @Test @Timeout(60)
    public void test_1() throws Exception {
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/projects/?EMextraParam123=42")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(9))
                .body("'collection'[0].'projectId'", numberMatches(1.0))
                .body("'collection'[0].'title'", containsString("TRANSBSCS"))
                .body("'collection'[0].'startDate'", containsString("28-09-2020"))
                .body("'collection'[0].'endDate'", containsString("04-11-2020"))
                .body("'collection'[0].'status'", containsString("COMPLETED"))
                .body("'collection'[1].'projectId'", numberMatches(2.0))
                .body("'collection'[1].'title'", containsString("SYNCH_BSCS_IMX"))
                .body("'collection'[1].'startDate'", containsString("26-11-2020"))
                .body("'collection'[1].'endDate'", containsString("25-03-2021"))
                .body("'collection'[1].'status'", containsString("IN_PROGRESS"))
                .body("'collection'[2].'projectId'", numberMatches(3.0))
                .body("'collection'[2].'title'", containsString("TASYI9A LILVIRANDA"))
                .body("'collection'[2].'startDate'", containsString("26-11-2020"))
                .body("'collection'[2].'endDate'", containsString("26-11-2020"))
                .body("'collection'[2].'status'", containsString("COMPLETED"))
                ; // Skipping assertions on the remaining 6 elements. This limit of 3 elements can be increased in the configurations
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-2"></a>
<details open>
<summary><b>test_2</b></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/locations
    */
    @Test @Timeout(60)
    public void test_2() throws Exception {
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/locations")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(2))
                .body("'collection'[0].'locationId'", numberMatches(1.0))
                .body("'collection'[0].'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[0].'postalCode'", containsString("2016"))
                .body("'collection'[0].'city'", containsString("LAC2"))
                .body("'collection'[1].'locationId'", numberMatches(2.0))
                .body("'collection'[1].'adr'", containsString("RUE DE BLA BLA"))
                .body("'collection'[1].'postalCode'", containsString("2016"))
                .body("'collection'[1].'city'", containsString("CHARGUIA"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-3"></a>
<details open>
<summary><b>test_3</b></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/locations
    */
    @Test @Timeout(60)
    public void test_3() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("LOCATIONS", 132L)
                .d("ADR", "\"SRMAyukXg0HOu\"")
                .d("POSTAL_CODE", "\"Eb\"")
                .d("CITY", "\"g6mwaokX1VPcWa\"")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/locations?" + 
                    "password=z&" + 
                    "username=QIzP_Pi6uBD")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(3))
                .body("'collection'[0].'locationId'", numberMatches(1.0))
                .body("'collection'[0].'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[0].'postalCode'", containsString("2016"))
                .body("'collection'[0].'city'", containsString("LAC2"))
                .body("'collection'[1].'locationId'", numberMatches(2.0))
                .body("'collection'[1].'adr'", containsString("RUE DE BLA BLA"))
                .body("'collection'[1].'postalCode'", containsString("2016"))
                .body("'collection'[1].'city'", containsString("CHARGUIA"))
                .body("'collection'[2].'locationId'", numberMatches(3.0))
                .body("'collection'[2].'adr'", containsString("SRMAyukXg0HOu"))
                .body("'collection'[2].'postalCode'", containsString("Eb"))
                .body("'collection'[2].'city'", containsString("g6mwaokX1VPcWa"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-4"></a>
<details open>
<summary><b>test_4</b></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/departments
    */
    @Test @Timeout(60)
    public void test_4() throws Exception {
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .get(baseUrlOfSut + "/app/api/departments")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(3))
                .body("'collection'[0].'departmentId'", numberMatches(4.0))
                .body("'collection'[0].'departmentName'", containsString("DWH"))
                .body("'collection'[0].'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[0].'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[0].'location'.'postalCode'", containsString("2016"))
                .body("'collection'[0].'location'.'city'", containsString("LAC2"))
                .body("'collection'[1].'departmentId'", numberMatches(5.0))
                .body("'collection'[1].'departmentName'", containsString("Digital"))
                .body("'collection'[1].'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[1].'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[1].'location'.'postalCode'", containsString("2016"))
                .body("'collection'[1].'location'.'city'", containsString("LAC2"))
                .body("'collection'[2].'departmentId'", numberMatches(6.0))
                .body("'collection'[2].'departmentName'", containsString("Billing"))
                .body("'collection'[2].'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[2].'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[2].'location'.'postalCode'", containsString("2016"))
                .body("'collection'[2].'location'.'city'", containsString("LAC2"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-5"></a>
<details open>
<summary><b>test_5</b></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/departments/
    */
    @Test @Timeout(60)
    public void test_5() throws Exception {
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "42")
                .get(baseUrlOfSut + "/app/api/departments/?EMextraParam123=42")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(3))
                .body("'collection'[0].'departmentId'", numberMatches(4.0))
                .body("'collection'[0].'departmentName'", containsString("DWH"))
                .body("'collection'[0].'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[0].'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[0].'location'.'postalCode'", containsString("2016"))
                .body("'collection'[0].'location'.'city'", containsString("LAC2"))
                .body("'collection'[1].'departmentId'", numberMatches(5.0))
                .body("'collection'[1].'departmentName'", containsString("Digital"))
                .body("'collection'[1].'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[1].'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[1].'location'.'postalCode'", containsString("2016"))
                .body("'collection'[1].'location'.'city'", containsString("LAC2"))
                .body("'collection'[2].'departmentId'", numberMatches(6.0))
                .body("'collection'[2].'departmentName'", containsString("Billing"))
                .body("'collection'[2].'location'.'locationId'", numberMatches(1.0))
                .body("'collection'[2].'location'.'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[2].'location'.'postalCode'", containsString("2016"))
                .body("'collection'[2].'location'.'city'", containsString("LAC2"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-6"></a>
<details open>
<summary><b>test_6</b></summary>

```java
    /**
    * Calls:
    * (200) DELETE:/app/api/employees/delete/{id}
    */
    @Test @Timeout(60)
    public void test_6() throws Exception {
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .delete(baseUrlOfSut + "/app/api/employees/delete/1?EMextraParam123=42")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body(containsString("true"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-7"></a>
<details open>
<summary><b>test_7</b></summary>

```java
    /**
    * Calls:
    * (200) DELETE:/app/api/credentials/username/{username}
    */
    @Test @Timeout(60)
    public void test_7() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .delete(baseUrlOfSut + "/app/api/credentials/username/NCv5HanSYi")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body(containsString("true"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-8"></a>
<details open>
<summary><b>test_8</b></summary>

```java
    /**
    * Calls:
    * (200) DELETE:/app/api/employees/username/{username}
    */
    @Test @Timeout(60)
    public void test_8() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .delete(baseUrlOfSut + "/app/api/employees/username/admin")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body(containsString("true"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-9"></a>
<details open>
<summary><b>test_9</b></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/credentials
    */
    @Test @Timeout(60)
    public void test_9() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .get(baseUrlOfSut + "/app/api/credentials")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(14))
                .body("'collection'[0].'credentialId'", numberMatches(1.0))
                .body("'collection'[0].'username'", containsString("imentouk"))
                .body("'collection'[0].'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[0].'enabled'", equalTo(true))
                .body("'collection'[0].'role'", containsString("ROLE_EMP"))
                .body("'collection'[1].'credentialId'", numberMatches(2.0))
                .body("'collection'[1].'username'", containsString("badridoudi"))
                .body("'collection'[1].'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[1].'enabled'", equalTo(true))
                .body("'collection'[1].'role'", containsString("ROLE_EMP"))
                .body("'collection'[2].'credentialId'", numberMatches(3.0))
                .body("'collection'[2].'username'", containsString("selimhorri"))
                .body("'collection'[2].'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[2].'enabled'", equalTo(true))
                .body("'collection'[2].'role'", containsString("ROLE_EMP"))
                ; // Skipping assertions on the remaining 11 elements. This limit of 3 elements can be increased in the configurations
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-10"></a>
<details open>
<summary><b>test_10</b></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/credentials/
    */
    @Test @Timeout(60)
    public void test_10() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .get(baseUrlOfSut + "/app/api/credentials/")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(14))
                .body("'collection'[0].'credentialId'", numberMatches(1.0))
                .body("'collection'[0].'username'", containsString("imentouk"))
                .body("'collection'[0].'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[0].'enabled'", equalTo(true))
                .body("'collection'[0].'role'", containsString("ROLE_EMP"))
                .body("'collection'[1].'credentialId'", numberMatches(2.0))
                .body("'collection'[1].'username'", containsString("badridoudi"))
                .body("'collection'[1].'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[1].'enabled'", equalTo(true))
                .body("'collection'[1].'role'", containsString("ROLE_EMP"))
                .body("'collection'[2].'credentialId'", numberMatches(3.0))
                .body("'collection'[2].'username'", containsString("selimhorri"))
                .body("'collection'[2].'password'", containsString("$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2"))
                .body("'collection'[2].'enabled'", equalTo(true))
                .body("'collection'[2].'role'", containsString("ROLE_EMP"))
                ; // Skipping assertions on the remaining 11 elements. This limit of 3 elements can be increased in the configurations
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-11"></a>
<details open>
<summary><b>test_11</b></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/projects/{id}
    */
    @Test @Timeout(60)
    public void test_11() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .get(baseUrlOfSut + "/app/api/projects/2")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'projectId'", numberMatches(2.0))
                .body("'title'", containsString("SYNCH_BSCS_IMX"))
                .body("'startDate'", containsString("26-11-2020"))
                .body("'endDate'", containsString("25-03-2021"))
                .body("'status'", containsString("IN_PROGRESS"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-12"></a>
<details open>
<summary><b>test_12</b></summary>

```java
    /**
    * Calls:
    * (200) GET:/app/api/locations/
    */
    @Test @Timeout(60)
    public void test_12() throws Exception {
        List<InsertionDto> insertions = sql().insertInto("DEPARTMENTS", 172L)
                .d("DEPARTMENT_NAME", "\"cpnXGmm\"")
            .and().insertInto("EMPLOYEES", 171L)
                .d("FIRST_NAME", "\"OuUVfBi\"")
                .d("LAST_NAME", "\"3BpLkuXewP\"")
                .d("EMAIL", "\"kmq@XOy.xaOW\"")
                .d("PHONE", "\"KqYqq6yxQGHPhJ\"")
                .d("JOB", "\"P_PF\"")
                .d("SALARY", "0.6355311891588135")
            .and().insertInto("DEPARTMENTS", 169L)
                .d("DEPARTMENT_NAME", "\"r\"")
            .and().insertInto("EMPLOYEES", 168L)
                .d("FIRST_NAME", "\"v9P3zZgDobCgg\"")
                .d("LAST_NAME", "\"3ZaAsO46b5p9ZWm\"")
                .d("EMAIL", "\"IngZ@W.wW\"")
                .d("PHONE", "\"OxFfX5XkXQrRoWV\"")
                .d("JOB", "\"4qox3baWf3tp\"")
                .d("SALARY", "0.4890975015973792")
            .and().insertInto("LOCATIONS", 167L)
                .d("ADR", "\"SeExk2L\"")
                .d("POSTAL_CODE", "\"bENRo6FTuZxueSZO\"")
                .d("CITY", "\"oD4qBBKgR76wmt\"")
            .and().insertInto("DEPARTMENTS", 166L)
                .d("DEPARTMENT_NAME", "\"QuN9\"")
            .and().insertInto("EMPLOYEES", 165L)
                .d("FIRST_NAME", "\"oHM1Ef\"")
                .d("LAST_NAME", "\"F0aW24AQ3s\"")
                .d("EMAIL", "\"FF@AU.ReBT\"")
                .d("PHONE", "\"ehJiZp4n\"")
                .d("JOB", "\"8cbnJvl_kTGAyME9\"")
                .d("SALARY", "0.042795373541171244")
            .and().insertInto("ASSIGNMENTS", 164L)
                .d("EMPLOYEE_ID", "13")
                .d("PROJECT_ID", "7")
                .d("COMMIT_DATE", "\"1965-05-04 06:17:30\"")
                .d("COMMIT_EMP_DESC", "\"oM\"")
                .d("COMMIT_MGR_DESC", "\"\"")
            .dtos();
        InsertionResultsDto insertionsresult = controller.execInsertionsIntoDatabase(insertions);
        
        final Map<String,String> cookies_ROLE_EMP = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=selimhorri&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_EMP)
                .get(baseUrlOfSut + "/app/api/locations/?" + 
                    "password=U73MT5RTL_bxNmX&" + 
                    "username=4e1s3IUcM")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'collection'.size()", equalTo(3))
                .body("'collection'[0].'locationId'", numberMatches(1.0))
                .body("'collection'[0].'adr'", containsString("RUE DE LA BOURSE"))
                .body("'collection'[0].'postalCode'", containsString("2016"))
                .body("'collection'[0].'city'", containsString("LAC2"))
                .body("'collection'[1].'locationId'", numberMatches(2.0))
                .body("'collection'[1].'adr'", containsString("RUE DE BLA BLA"))
                .body("'collection'[1].'postalCode'", containsString("2016"))
                .body("'collection'[1].'city'", containsString("CHARGUIA"))
                .body("'collection'[2].'locationId'", numberMatches(3.0))
                .body("'collection'[2].'adr'", containsString("SeExk2L"))
                .body("'collection'[2].'postalCode'", containsString("bENRo6FTuZxueSZO"))
                .body("'collection'[2].'city'", containsString("oD4qBBKgR76wmt"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-13"></a>
<details open>
<summary><b>test_13</b></summary>

```java
    /**
    * Calls:
    * (200) PUT:/app/api/locations
    */
    @Test @Timeout(60)
    public void test_13() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" { " + 
                    " \"adr\": \"V4ANdj_0Yja01Ka\", " + 
                    " \"city\": \"Ok3kQXdJOldgGJ\", " + 
                    " \"postalCode\": \"sfSsn\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/locations")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'locationId'", numberMatches(3.0))
                .body("'adr'", containsString("V4ANdj_0Yja01Ka"))
                .body("'postalCode'", containsString("sfSsn"))
                .body("'city'", containsString("Ok3kQXdJOldgGJ"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-14"></a>
<details open>
<summary><b>test_14</b></summary>

```java
    /**
    * Calls:
    * (200) POST:/app/api/locations/save
    */
    @Test @Timeout(60)
    public void test_14() throws Exception {
        
        final Map<String,String> cookies_ROLE_MGR = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=soumayahajjem&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_MGR)
                .contentType("application/json")
                .body(" { " + 
                    " \"adr\": \"Y8fQj\", " + 
                    " \"city\": \"JhBmar\", " + 
                    " \"locationId\": 10106611, " + 
                    " \"postalCode\": \"MHZa\" " + 
                    " } ")
                .post(baseUrlOfSut + "/app/api/locations/save")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'locationId'", numberMatches(4.0))
                .body("'adr'", containsString("Y8fQj"))
                .body("'postalCode'", containsString("MHZa"))
                .body("'city'", containsString("JhBmar"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-15"></a>
<details open>
<summary><b>test_15</b></summary>

```java
    /**
    * Calls:
    * (200) PUT:/app/api/credentials
    */
    @Test @Timeout(60)
    public void test_15() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" { " + 
                    " \"credentialId\": 516, " + 
                    " \"enabled\": false, " + 
                    " \"password\": \"$2a$10$6pNV34gbMAEj6vuyVmQMdOfSKk.kuxOUOeucg78/cvOprSR3lsZL2\", " + 
                    " \"role\": \"cQOySXQt0Ew\", " + 
                    " \"username\": \"NCv5HanSYi\" " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/credentials")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'credentialId'", numberMatches(15.0))
                .body("'username'", containsString("NCv5HanSYi"))
                .body("'password'", containsString("$2a$10$FrNH3z7hZ3eExguIz90fL.u0cjP.xKwqJxtpr7Au7kKu453LvE9GS"))
                .body("'enabled'", equalTo(false))
                .body("'role'", containsString("cQOySXQt0Ew"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>

<a name="test-successes-java-test-16"></a>
<details open>
<summary><b>test_16</b></summary>

```java
    /**
    * Calls:
    * (200) PUT:/app/api/departments/update
    */
    @Test @Timeout(60)
    public void test_16() throws Exception {
        
        final Map<String,String> cookies_ROLE_ADMIN = given()
            .contentType("application/x-www-form-urlencoded")
            .body("username=admin&password=test")
            .post(baseUrlOfSut + "/app/login")
            .then().extract().cookies();
            
        
        given().accept("*/*")
                .header("x-EMextraHeader123", "")
                .cookies(cookies_ROLE_ADMIN)
                .contentType("application/json")
                .body(" { " + 
                    " \"departmentId\": -793207560, " + 
                    " \"departmentName\": \"hWf4qKIK5\", " + 
                    " \"location\": { " + 
                    " \"adr\": \"YBmBONGS_lC3od\", " + 
                    " \"city\": \"_EM_675_XYZ_\", " + 
                    " \"locationId\": 2 " + 
                    " } " + 
                    " } ")
                .put(baseUrlOfSut + "/app/api/departments/update")
                .then()
                .statusCode(200)
                .assertThat()
                .contentType("application/json")
                .body("'departmentId'", numberMatches(3.0))
                .body("'departmentName'", containsString("hWf4qKIK5"))
                .body("'location'.'locationId'", numberMatches(2.0))
                .body("'location'.'adr'", containsString("RUE DE BLA BLA"))
                .body("'location'.'postalCode'", containsString("2016"))
                .body("'location'.'city'", containsString("CHARGUIA"));
    }
```

[&#x2191; back to faults](#user-content-wfc-faults)

</details>
