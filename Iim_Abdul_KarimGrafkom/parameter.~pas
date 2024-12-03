unit parameter;

interface

uses
  Windows, Messages, SysUtils, Variants, Classes, Graphics, Controls, Forms,
  Dialogs, StdCtrls;

type
  TForm1 = class(TForm)
    Button1: TButton;
    Button2: TButton;
    Button3: TButton;
    procedure Button1Click(Sender: TObject);
    procedure Button2Click(Sender: TObject);
    procedure Button3Click(Sender: TObject);
  private
    { Private declarations }
  public
    { Public declarations }
  end;

var
  Form1: TForm1;

implementation

{$R *.dfm}

procedure TForm1.Button1Click(Sender: TObject);
var fs,fy: real; 
    x:integer; 
begin 
    fs:=0.0;
    for x:=0 to 740 do
    begin
    fy:=80*sin(fs/40);
   canvas.pixels[trunc(320+fs),trunc(240-fy)]:=clred;
   canvas.pixels[trunc(320-fs),trunc(240-fy)]:=clred;
    fs:=fs+1;
end;
end;
procedure TForm1.Button2Click(Sender: TObject);
var r,d,c,x,y,theta,thetf: real; 
    a,xc,yc:integer; 
begin 
     a:=100;xc:=300;yc:=200; 
     thetf:=0.0; 
   d:=2*PI; 
   theta:=d; 
   c:=1/a; 
 while (thetf<theta) do 
 begin 
       r:=a*cos(3*thetf); 
       x:=r*cos(thetf); 
       y:=-r*sin(thetf); 
       canvas.pixels[trunc(xc+x),trunc(yc+y)]:=clblue; 
       thetf:=thetf+c; 
end; 
end; 
procedure TForm1.Button3Click(Sender: TObject);
var r,d,c,x,y,theta,thetf: real; 
a,xc,yc:integer; 
begin 
     a:=50;xc:=300;yc:=100; 
     thetf:=0.0; 
     d:=2*PI; 
     theta:=d; 
     c:=1/a; 
    while (thetf<theta) do 
    begin 
    r:=a*thetf; 
    x:=r*cos(thetf); 
    y:=-r*sin(thetf); 
canvas.pixels[trunc(xc+x),trunc(yc+y)]:=clblue; 
thetf:=thetf+c; 
end; 
end; 
end.



