![C++](https://img.shields.io/badge/language-C++-00599C?logo=c%2B%2B&logoColor=white)

# Dangerous Function Filter 

A list of blocked / dangerous functions that you can add to your namecallhooks/metahooks for your internal executor.


Check the filter >
```cpp
inline static bool IsFunctionRestricted(const char* name)
{
    return RestrictedFunctionCalls.count(to_lower(name)) != 0;
}

inline static bool IsRestrictedService(const char* name)
{
    return RstrictedServiceCalls.count(to_lower(name)) != 0;
}```
