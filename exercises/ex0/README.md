# Getting Started

In this exercise, you will get to know a few user credentials that you need to remember throughout this session. Please do not use any other user other than the one intended for you. 

## Your needed users

There's only two users that you need in the entire session. Both of them are provided by SAP, please do not use your personal users for the subsequent exercises.

1.	Since you will be using an extension application for an SAP S/4HANA on-premise system, you'll obviously need a user to ju.
<br>![](/exercises/ex0/images/00_00_0010.png)

2.	Insert this code.
``` abap
 DATA(params) = request->get_form_fields(  ).
 READ TABLE params REFERENCE INTO DATA(param) WITH KEY name = 'cmd'.
  IF sy-subrc <> 0.
    response->set_status( i_code = 400
                     i_reason = 'Bad request').
    RETURN.
  ENDIF.
```

## Summary

Now that you have ... 
Continue to - [Exercise 1 - Exercise 1 Description](../ex1/README.md)
