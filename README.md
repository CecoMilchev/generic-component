# generic-component

A repository showcasing the need to specify TItem when a generic component is used. 

As of .NET 7 prev 5 and newer, when a generic component has an `EventCallback<GenericComponentEventArgs<TItem>>`, a compiler error is thrown stating:

> _The type or namespace name 'TItem' could not be found (are you missing a using directive or an assembly reference?)_

To resolve this, the TItem attribute should be explicitly specified for the generic component. 