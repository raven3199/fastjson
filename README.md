# CS304 Progress Proposal

### Group Name: Gangsters

### Group Member:

- 薛嘉诚 11911402
- 于佳宁 11911406
- 李怀武 11911425
- 张润东 11911426
- 田荫熙 21990006

### Group Project: Fastjson



## (a) Issues we have selected and Reasons

- Issue #4069 (link: https://github.com/alibaba/fastjson/issues/4069)

  Reason: It relates to the validation check of `String` in `JSON` form. It is a good and easy start for us to learn the structure of serialization and deserialization. So, we choose to work on it first. On the other hand, the cause of the problem is clear because the person committed issue also provide how to reconstruct the problem scene. As a result, it is easy and clear to build test cases.

- Issue #4009 (link: https://github.com/alibaba/fastjson/issues/4009)

  Reason: After learning the basic process of serialization and deserialization, this issue is suitable for dealing with serialization actually. It relates to the deserialization of `HashMap` and the features of building output stream. Moreover, it is also clear to reconstruct the scene of issue and build test cases.



## (b) Test scenarios for each issue.

- Issue #4069 (link: https://github.com/alibaba/fastjson/issues/4069)

  - Scenario 1: When validating an array with arrays inside it using the method `isValidArray()`, the result of whether it is valid array is `False`.
  - Scenario 2: When validating above array in another way `JSONValidator.getType()`, the result of the type of this string is `Array`.

- Issue #4009 (link: https://github.com/alibaba/fastjson/issues/4009)

  - Scenario 1: When changing `HashMap` into `JSON`, it will arise problems when taking `UUID` as the key and with feature `BrowserSecure`. The problem will be that there will be a duplicate pair of `""` outside the `UUID`.

  - Scenario 2: For above scenario, if changing without feature `BrowserSecure`, there will be no problem arise.



## (c) Pull Request for each issue

- Issue #4069: PR link: https://github.com/alibaba/fastjson/pull/4087
- Issue #4009: PR link: https://github.com/alibaba/fastjson/pull/4094



## (g) Future schedule

|  Time   |               Schedule                |
| :-----: | :-----------------------------------: |
| Week 12 |   Choosing two issues and fix them    |
| Week 13 |   Choosing two issues and fix them    |
| Week 14 |     Choosing one issue and fix it     |
| Week 15 | Reserved time for unexpected problems |



## (h) Lab session

We decide to take part in lab session 1. Choosing **TA A** for **Slot 2**. The decision has been recorded in GitHub Projects2022.