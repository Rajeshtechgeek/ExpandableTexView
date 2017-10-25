# ExpandableTexView
This is an Android Expandable Textview which can be  fully customisable for your needs.

 Use xml code below 
 
 <YourPackage.ExpandableTextView                     
 android:layout_marginLeft="16dp"                    
 android:layout_marginRight="16dp"                    
 android:id="@+id/event_description"                    
 android:layout_width="wrap_content"                    
 android:layout_height="wrap_content"                                     
 android:text="Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus." />
 
 
 And in your Activity:
 
 eventDescription = view.findViewById(R.id.event_description);
 eventDescription.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                if(eventDescription.isExpanded()){
                    eventDescription.truncateText();
                }else {
                    eventDescription.expandText();
                }
            }
        });
