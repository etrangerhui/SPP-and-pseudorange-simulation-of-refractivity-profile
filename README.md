Using ray tracing technique to do GPS positioning
Run CRinex.exe, open-madr2000.06o and open Navi-brdc2000.06n
Edit/SPP do location, choose Custom Profile or Fix position/Drift profile with or withou tropshere and ionosphere correction
     Custom profile: define 10km to -27000km height refractivity(N=n*1.e6-1)
                Insert key to insert a node like 0 km, -12km for tropsphere top, -350km for ionsphere 
                Del Key to delete a node, don't delete 10km and -27000km node
     Custom profile with all 0 refractivity is linear ray tracing,can bined with tropsphere and ionosphere correction
               if you really choose defined your own profile, please uncheck both corrections
     Click OK to show the {XYZ,DT} curvers minus their average(shown at the bottom together with variance)
Edit/Psudorange to calculate theoretical one by CRinex, then do SPP with you conbinations
Note: only GPS C1,P1,P2 channel supported, different channel only affected by ionosphere correction
      for P1&P2 dual channel, the observation is linear conbinated to remove ionosherical effect. 
      for dual channel,P1 was treated as 1575.42e6, C1 was treated as -1575.42e6, P2 was treated 1227.6e6 
