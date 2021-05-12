# cs0x7f_min2phase_CSharp
A C# version of Chen Shuang's java version of Rubik's Cube solver or scrambler,  under .NET Core 3.1.

Chen Shuang's optimized implementation of Kociemba's two-phase algorithm can be found here:https://github.com/cs0x7f/min2phase.
All credit for this solution goes to him.

I tried my best to translate the original code. All work fine. The only regret is the C# version dose not run much faster then the Java version.  

Some necessary language adaption between Java and C# is made. 

1.Jagged Arrays can be initialized in Java when defined. But in C#, they are moved to the class constructor to finish the initialization. 

For example:

            //static char[][] UDSliceMove = new char[N_SLICE][N_MOVES];
            
            public static char[][] UDSliceMove = new char[N_SLICE][];
            
            for (int i = 0; i < N_SLICE; i++)
            
            {
            
                UDSliceMove[i] = new char[N_MOVES];
                
            }
            
2.The ui MainProgram in Java version is changed to WPF App(NET).

3....
