

## Entropy in software

The idea

Chaos monkey for code. This tool helps you by deleting some code from your git repository. The unit of granularity of the deletion is a function or method.
In scala we are going to implement this via an sbt plugin.

The idea of the project is twofold, on one side, it would be interesting to see how the code evolves over time when removing 
code, we envisage that large functions or methods will be penalized, as it will be harder to rewrite


## 

- the sbt plugin should:
    - run periodically (configurable) on build server.
    - run some static analisys tool (that will measure code cohesion and other metrics).    
    - checkout a repo
    - remove some code and run the build (special criteria??)
    - collect information about what was deleted and what was the failure.    
    - push notifications about the deletion results (what was deleted, build result, etc).


