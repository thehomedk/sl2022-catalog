<script lang="ts">
  export let strings: Record<string, string>
  export let locationId: string
  export let identifier: number

  if (identifier === 1406 || identifier === 1414) {
    locationId = 'skate'
  }

  if (identifier === 1362) {
    locationId = 'swim'
  }

  if (identifier === 1405) {
    locationId = 'kroppedal'
  }

  const schedules = {
    a14: {
      outText: strings.a14outText,
      backText: strings.backText,
      out: [
        {
          name: 'monday',
          departures: ['8:30', '', '13:00', '16:00', '18:30'],
        },
        {
          name: 'tuesday',
          departures: ['8:30', '', '13:00', '16:00', '18:30'],
        },
        {
          name: 'wednesday',
          departures: ['8:30', '', '13:00', '16:00', ''],
        },
        {
          name: 'thursday',
          departures: ['8:30', '11:30', '13:00', '16:00', ''],
        },
        {
          name: 'friday',
          departures: ['8:30', '', '13:00', '16:00', ''],
        },
      ],
      back: [
        {
          name: 'monday',
          departures: ['12:00', '16:30', '17:30', '22:00', '23:00'],
        },
        {
          name: 'tuesday',
          departures: ['12:00', '16:30', '', '22:00', '23:00'],
        },
        {
          name: 'wednesday',
          departures: ['12:00', '16:30', '17:30', '', ''],
        },
        {
          name: 'thursday',
          departures: ['12:00', '16:30', '17:30', '', ''],
        },
        {
          name: 'friday',
          departures: ['12:00', '16:30', '17:30', '', ''],
        },
      ],
    },

    a13: {
      outText: strings.a13outText,
      backText: strings.backText,
      out: [
        {
          name: 'sunday',
          departures: ['', '', '13:00', '17:00'],
        },
        {
          name: 'monday',
          departures: ['8:30', '', '13:00', '17:00'],
        },
        {
          name: 'tuesday',
          departures: ['8:30', '11:30', '13:00', '17:00'],
        },
        {
          name: 'wednesday',
          departures: ['8:30', '11:30', '13:00', '17:00'],
        },
        {
          name: 'thursday',
          departures: ['8:30', '11:30', '13:00', '17:00'],
        },
        {
          name: 'friday',
          departures: ['8:30', '11:30', '13:00', '17:00'],
        },
        {
          name: 'saturday',
          departures: ['8:30', '', '', ''],
        },
      ],
      back: [
        {
          name: 'sunday',
          departures: ['', '16:30', '17:30', ''],
        },
        {
          name: 'monday',
          departures: ['12:00', '16:30', '17:30', '22:00'],
        },
        {
          name: 'tuesday',
          departures: ['12:00', '16:30', '17:30', ''],
        },
        {
          name: 'wednesday',
          departures: ['12:00', '16:30', '17:30', ''],
        },
        {
          name: 'thursday',
          departures: ['12:00', '16:30', '17:30', ''],
        },
        {
          name: 'friday',
          departures: ['12:00', '16:30', '17:30', ''],
        },
        {
          name: 'saturday',
          departures: ['12:00', '15:00', '', ''],
        },
      ],
    },

    a12: {
      outText: strings.a12outText,
      backText: strings.backText,
      out: [
        {
          name: 'monday',
          departures: ['7:30', '8:30', strings.halfHourly, '20:30', '21:30'],
        },
        {
          name: 'tuesday',
          departures: ['7:30', '8:30', strings.halfHourly, '20:30', '21:30'],
        },
        {
          name: 'wednesday',
          departures: ['7:30', '8:30', strings.halfHourly, '20:30', '21:30'],
        },
        {
          name: 'thursday',
          departures: ['7:30', '8:30', strings.halfHourly, '20:30', '21:30'],
        },
        {
          name: 'friday',
          departures: ['7:30', '8:30', strings.halfHourly, '20:30', '21:30'],
        },
      ],
      back: [
        {
          name: 'monday',
          departures: ['8:00', '9:00', strings.halfHourly, '21:00', '22:00'],
        },
        {
          name: 'tuesday',
          departures: ['8:00', '9:00', strings.halfHourly, '21:00', '22:00'],
        },
        {
          name: 'wednesday',
          departures: ['8:00', '9:00', strings.halfHourly, '21:00', '22:00'],
        },
        {
          name: 'thursday',
          departures: ['8:00', '9:00', strings.halfHourly, '21:00', '22:00'],
        },
        {
          name: 'friday',
          departures: ['8:00', '9:00', strings.halfHourly, '21:00', '22:00'],
        },
      ],
    },

    kroppedal: {
      outText: strings.kroppedaloutText,
      backText: strings.backText,
      out: [
        {
          name: 'monday',
          departures: ['11:30', '13:00'],
        },
        {
          name: 'tuesday',
          departures: ['11:30', '13:00'],
        },
        {
          name: 'wednesday',
          departures: ['11:30', '13:00'],
        },
        {
          name: 'thursday',
          departures: ['11:30', '13:00'],
        },
        {
          name: 'friday',
          departures: ['11:30', '13:00'],
        },
      ],
      back: [
        {
          name: 'monday',
          departures: ['13:30', '15:00'],
        },
        {
          name: 'tuesday',
          departures: ['13:30', '15:00'],
        },
        {
          name: 'wednesday',
          departures: ['13:30', '15:00'],
        },
        {
          name: 'thursday',
          departures: ['13:30', '15:00'],
        },
        {
          name: 'friday',
          departures: ['13:30', '15:00'],
        },
      ],
    },

    skate: {
      outText: strings.skateoutText,
      backText: strings.backText,
      out: [
        {
          name: 'monday',
          departures: ['11:30', '13:00'],
        },
        {
          name: 'tuesday',
          departures: ['11:30', '13:00'],
        },
        {
          name: 'wednesday',
          departures: ['11:30', '13:00'],
        },
        {
          name: 'thursday',
          departures: ['11:30', '13:00'],
        },
        {
          name: 'friday',
          departures: ['11:30', '13:00'],
        },
      ],
      back: [
        {
          name: 'monday',
          departures: ['14:00', '15:30'],
        },
        {
          name: 'tuesday',
          departures: ['14:00', '15:30'],
        },
        {
          name: 'wednesday',
          departures: ['14:00', '15:30'],
        },
        {
          name: 'thursday',
          departures: ['14:00', '15:30'],
        },
        {
          name: 'friday',
          departures: ['14:00', '15:30'],
        },
      ],
    },

    swim: {
      outText: strings.swimoutText,
      backText: strings.backText,
      out: [
        {
          name: 'monday',
          departures: ["9:30", "10:30", "11:30", "12:30", "13:30", "14:30"]
        },
        {
          name: 'tuesday',
          departures: ["9:30", "10:30", "11:30", "12:30", "13:30", "14:30"]
        },
        {
          name: 'wednesday',
          departures: ["9:30", "10:30", "11:30", "12:30", "13:30", "14:30"]
        },
        {
          name: 'thursday',
          departures: ["9:30", "10:30", "11:30", "12:30", "13:30", "14:30"]
        },
        {
          name: 'friday',
          departures: ["9:30", "10:30", "11:30", "12:30", "13:30", "14:30"]
        },
      ],
      back: [
        {
          name: 'monday',
          departures: [ "12:00", "13:00", "14:00", "15:00", "16:00", "17:00"]	
        },
        {
          name: 'tuesday',
          departures: [ "12:00", "13:00", "14:00", "15:00", "16:00", "17:00"]	
        },
        {
          name: 'wednesday',
          departures: [ "12:00", "13:00", "14:00", "15:00", "16:00", "17:00"]	
        },
        {
          name: 'thursday',
          departures: [ "12:00", "13:00", "14:00", "15:00", "16:00", "17:00"]	
        },
        {
          name: 'friday',
          departures: [ "12:00", "13:00", "14:00", "15:00", "16:00", "17:00"]	
        },
      ],
    },
  }
</script>

{#if locationId === 'skate'}
<div class="font-bold text-red-500">{strings.scheduleNotice}</div>
{/if}

{#if schedules[locationId]}
  <div class="mb-1 text-base font-semibold">{strings.transport_info}</div>
  <div class="flex flex-col gap-x-4 gap-y-4 sm:flex-row sm:gap-y-0">
    <table class="table-auto border-2">
      <tr class="bg-blue-200">
        <td class="border-b-2 p-1" colspan="7">{schedules[locationId].outText}</td>
      </tr>
      {#each schedules[locationId].out as day, index}
        {@const even = index % 2 === 0}
        <tr class:bg-gray-100={even}>
          <td class="p-1">{strings[day.name]}</td>
          {#each day.departures as departure}
            <td class="whitespace-nowrap p-1">{departure}</td>
          {/each}
        </tr>
      {/each}
    </table>
    <table class="table-auto border-2">
      <tr class="bg-blue-200">
        <td class="border-b-2 p-1" colspan="7">{schedules[locationId].backText}</td>
      </tr>
      {#each schedules[locationId].back as day, index}
        {@const even = index % 2 === 0}
        <tr class:bg-gray-100={even}>
          <td class="p-1">{strings[day.name]}</td>
          {#each day.departures as departure}
            <td class="whitespace-nowrap p-1">{departure}</td>
          {/each}
        </tr>
      {/each}
    </table>
  </div>
{/if}
