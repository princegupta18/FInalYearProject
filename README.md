# Plan
```
1. Develop training module.
    1.1 Make it load a tensorflow pose model (PoseNet, MoveNet or BlazePose)
    1.2 Test model limitations (Occulsions, Lighting, Partial Body Parts, Angles)
    1.3 Create a table of different tests
    1.4 Create interface for the basic exercise model training
        Models:
        1) "A" Pose
        2) Model 1: Standing, Squat or Planche
        3) Model 2: Standing -> Guard?, Standing -> Squat?
        4) Model 3: Guard -> Jab, Guard -> Cross
        5) Model 4: Squat -> Up, Squat -> Down  
        6) 

    1.5 Turn all the Tensorflow trained models to keras model(.h5) and then finally to protobuff file (.pb)

2. Develop the backend modules
    2.1 Be able to load the network stream objects into corresponding c++ data structure
    2.2 Use the models trained from Step 1 to predict this data.
    2.3 Store the data from 2.2 to storage (now implemented as mongoDB)
    2.4 
```