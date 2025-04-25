# Directive
Directive  Component

<P [ngClass]="myclass">dem-directives works!</P>



<p [ngClass]="{'custom-style':isCustom,'Custom-block':!isCustom}"> condition baxsed class</p>

<p style="display :block; color:rgb(21, 21, 211); background-color: yellow; font-size: 20px;">demo directives wors</p>

<p [ngStyle]="mystyle" style="font-size: 20px;">
  demo-dirctioves

</p>
<h2>structural dirctives </h2>
<div *ngIf="isCustomContent">
  <h3>
    this is Custom content
  </h3>
</div>
<div *ngIf="isCustomContent">
  <h3>this is Custom Content</h3>
</div>
<div *ngIf="isCustomIfelse; else CustomElse ">
  <h3>this is CUstom content</h3>
</div>
<ng-template #CustomElse>
  <div>
    <h3>this is else part of content </h3>
  </div>
  <div [ngSwitch]="days">
    <p *ngSwitchCase="'Monday'"> Today is Monday</p>
    <p *ngSwitchCase="'Tuesday'"> Today is Tuesday</p>
    <p *ngSwitchCase="'Wednessday'">Today is wednessday</p>
    <p *ngSwitchCase="'Thursday'">Today is Thursday</p>
    <p *ngSwitchCase="'Friday'">Today is Friday</p>
    <p *ngSwitchCase="'Saturday'">Today is Saturday</p>
    <p *ngSwitchCase="'Sunday'">Today is Sunday</p>

    <p *ngSwitchDefault>
      Day is not matched
    </p>







  </div>
  <h2>Ng for </h2>

  <p *ngFor="let item of  ['manohar','mukesh','Anil','Ajay','deepak'],let i=index ">index={{i}}and value:{{item}}</p>
  <div *ngFor="let items; let i=index">
    index={{i}},id={{item.id}},
    name={{item.name}}frofession{{item.profession}}
  </div>
</ng-template>


