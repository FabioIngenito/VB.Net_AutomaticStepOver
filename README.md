# VB.Net_AutomaticStepOver

When I was debugging step by step with "F11" for the first time in VS2013 he keeps giving this message:
Quando fui depurar passo a passo com "F11" pela primeira vez no VS2013 ele fica dando esta mensagem:

---------------------------
Microsoft Visual Studio
---------------------------
Your step-into request resulted in an automatic step-over of a property or operator.

This behavior can be overridden in the context menu for the line being executed by choosing 'Step Into Specific'  or by unchecking the option 'Step over properties and operators'.

Do you want to continue being notified when an automatic step-over happens?
---------------------------
Yes - Sim        No - Não   
---------------------------

SOLUTION:
SOLUÇÃO:

http://stackoverflow.com/questions/2672996/your-step-into-request-resulted-in-an-automatic-step-over-of-a-property-or-opera

- VS2010:
The setting for this in VS2010 is under: Tools -> Option -> Debugging (near the middle)

- VS2012:
There are three ways to change this behaviour in VS2012:
•Change the settings: Tools->Options->Debugging->General->Step over properties and operators OR
•Right click on the line of code to get the context menu. Then untick: Step over properties and operators OR
•Select 'Step into Specific' in the right click context menu which will ask you which specific function you would like to step into. It will list all the properties/functions involved in the current source line.

- VS2013:
Tools -> Option -> Debugging / General
* Step over properties and operators (Managed Only)

- VS2015:
Tools -> Option -> Debugging / General
* Step over properties and operators (Managed Only)
