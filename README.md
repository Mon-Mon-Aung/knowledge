# knowledge
knowledge

# Changing User Password using php artisan tinker
use App\Models\User;
use Illuminate\Support\Facades\Hash;

$admin = User::where('username', 'admin')->first();
$admin->password = Hash::make('newpassword');
$admin->save();
