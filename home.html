Laravel CMD installing 

1 > cd c:\ 

c:\> cd xampp\htdocs\my_new_laravel\



2   composer global require "laravel/installer"



3   composer create-project --prefer-dist laravel/laravel my_new_laravel


php artisan make:auth


php artisan migrate


routes


Route::post('insert-data', 'MyController@insertdata');
Route::get('home', 'MyController@get');
Route::post('update', 'MyController@updaterole');
Route::get('delet{id}', 'MyController@delet');



Controllers



<?php

//namespace App\Http\Controllers;

//use Illuminate\Http\Request;


namespace App\Http\Controllers;
use Illuminate\Support\Facades\Input;

use App\my_model;
use Request;
use DB;

//use App\Http\Requests;




class MyController extends Controller
{
    /**
     * Create a new controller instance.
     *
     * @return void
     */
    public function __construct()
    {
        $this->middleware('auth');
    }
	public function index()
    {
		$my_model = new my_model;
        return view('home');
    }
	public function insertdata(Request $request)
	{
		 $post=Request::all();
         //print_r($post);
         $uniq_id = uniqid();
		 $destinationPath ='public/uploads'; // upload path
		 $extension = Input::file('photo')->getClientOriginalExtension();
		 $fileName = rand(11111,99999).'.'.$extension; // renameing image
		 Input::file('photo')->move($destinationPath, $fileName); 
		

		  $data =array(  
     	                    'content_id' => $uniq_id, 
							'name' => $post['name'], 
							'photo' =>  $fileName,
							'sir' =>  $post['sir'], 		
							 						
                       ); 
					   
					$ck = DB::table('sir')->insert($data);
					
					return redirect()->back();
		
		 
	}
	public function get()
	{
		$adds = DB::table('sir')->get();

        return view('home', ['profileab' => $adds]);
	}
	
	public function updaterole(Request $request)
	{
		 $post=Request::all();
         //print_r($post);
         //$uniq_id = uniqid();
		 $destinationPath ='public/uploads'; // upload path
		 $extension = Input::file('photo')->getClientOriginalExtension();
		 $fileName = rand(11111,99999).'.'.$extension; // renameing image
		 Input::file('photo')->move($destinationPath, $fileName); 
		

		  $data =array(  
     	                    //'content_id' => $uniq_id, 
							'name' => $post['name'], 
							'photo' =>  $fileName,
							'sir' =>  $post['sir'], 		
							 						
                       ); 
					   
				$ck = DB::table('sir')->where('id',$post['id'])->update($data);
                   
           
           return redirect()->back();
	
	}
	
	public function delet($id)
	{
	         echo $id;
		     $data = my_model::find($id);
		     $data->delete($id);
		    
		     return redirect()->back();
	}
	
}




model

<?php
namespace App;

use IIIuminate\Database\Eloquent\Model;

class my_model extends Model 

{
    protected $table = "sir";
    //protected $fillable  = ['name', 'photo', 'sir'];
}
?>


view


<form action="insert-data" method="post" enctype="multipart/form-data" role="form">
                    {{ csrf_field() }}
					<table width="100%">
					<tr>
					<td>Name</td>
					<td><input type="text" name="name"></td>
					</tr>
					<tr>
					<td>file</td>
					<td><input type="file" name="photo"></td>
					</tr>
					<tr>
					<td>sir</td>
					<td><input type="text" name="sir"></td>
					</tr>
					<tr>
					<td><input type="submit" value="submit"></td>
					</tr>
					</table>
					</form>
					<br><br>
					<table width="100%">
					<tr>
					<td>Name</td>
					<td>file</td>
					<td>sir</td>
					<td>Action</td>
					</tr>
					@foreach($profileab as $row)
					<tr>
					<td><input type="text" name="name" value="{{$row->name}}"></td>
					<td><input type="file" name="photo"> &nbsp;<img src="{{ URL::to('/public') }}/uploads/{{$row->photo}}"width="50px"></td>
					<td><input type="text" name="sir" value="{{$row->sir}}"></td>

					<td><input type="button" value="update" data-toggle="modal" data-target="#myModal{{$row->name}}">&nbsp;<a href="delet{{$row->id}}"><input type="button" value="delete"></td>
					</tr>
					</form>