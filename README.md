# Dynamic Database Controls (ibcontrols)

The Dynamic Data Controls were originally distributed as an integral part of the 
IBX for Lazarus package and were dependent on the use of IBX for database access. 

Starting with IBX release 2.7.0, the “ibcontrols” package is no longer dependent on 
IBX. Pascal (corba) interfaces are used to communicate between the controls and the 
database access provider (e.g. IBX) and any similar package that provides the same 
interfaces can now be used with the controls. Developers of other Database Access 
Providers are encouraged to use these interfaces as defined in the code snippet 
IBDynamicInterfaces.inc and to provide the same functionality in their packages, and 
hence to allow their use with the Dynamic Database Controls.

The Lazarus IDE pallet tab for these controls has also been renamed from “Firebird Data Controls” 
to “Dynamic Database Controls”. The package name remains “ibcontrols”.

The Dynamic Database Controls are: 
    • TDBControlGrid           (Works with any Database Driver)
    • TIBDynamicGrid           (Other than dynamic row sorting works with any Database Driver)
    • TIBLookupComboEditBox    (Requires IBX or IBDynamicInterfaces support)
    • TIBTreeview              (Requires IBX or IBDynamicInterfaces support)
    • TIBArrayGrid             (Requires IBX or IBDynamicInterfaces support 
                                and specific to Firebird arrays)

For full information on the dynamic database controls and IBDynamicData interface see
the user guide in the doc directory.

All examples of use are provided by the IBX for Lazarus package which must be installed in
order to see the examples.
