                                                    ANGULAR App Component .HTML CODE
<header>
  <app-header></app-header>
</header>

<app-main-nav (sectionChange)="onSectionChange($event)"></app-main-nav>

<app-sidebar-left></app-sidebar-left>
<app-sidebar-right></app-sidebar-right>

<main>
  <app-home *ngIf="currentSection === 'home'"></app-home>
  <app-about *ngIf="currentSection === 'about'"></app-about>
  <app-courses *ngIf="currentSection === 'courses'"></app-courses>
  <app-apply *ngIf="currentSection === 'apply'"></app-apply>
  <app-student-info *ngIf="currentSection === 'student-info'"></app-student-info>
</main>

<footer>
  <p>&copy; 2024 Chanakya University. All rights reserved.</p>
</footer>
